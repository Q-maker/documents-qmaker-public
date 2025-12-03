# How to structure a TXT file to contain questions and answers for QcmMaker

The TXT files are structured to contain one or multiple **question-answer sections**. This guide is divided into two parts:

## 1. Standard Question-Answer Format

### 🧱 Basic Example
```
Among the following animals,
which of these animals lives in the water?
-Cat
-Dog
*Fish
-Horse
> Fish are aquatic animals that populate seas, oceans, rivers, ponds and water points.
```

### 📌 Rules
- A section begins with the **wording of the question**. It can span multiple lines.
- The proposed answers follow and must:
    - Be **true** if preceded by an asterisk `*`
    - Be **false** if preceded by a dash `-`
- A **comment/explanation** may follow, prefixed with `>` (optional).

### 📌 Multi-question Structure
- Each question section is separated by a **blank line** (i.e., two consecutive line returns).

### 🧾 Example with Two Questions
```
Among the following animals,
which of these animals lives in the water?
-Cat
-Dog
*Fish
-Horse
> Fish are aquatic animals that populate seas, oceans, rivers, ponds and water points.

Which of these animals are flying?
*Pigeon
-Dog
*Raven
*Eagle
> The pigeon, the raven and the eagle are all flying birds.
```

### ⚠️ Encoding Advice
For best compatibility, prefer saving your file in **UTF-8** encoding.

---

## 2. Advanced Configuration Options

QcmMaker allows much more than just basic formatting.
Below, we will discover  all advanced options supported via metadata.
The information below are more technical and is intended for advanced users!
First let start by an example of quiz with three questions:
```
@enumerate_all
List three animals found in a farmyard:
*chicken
*duck
*turkey
> These three animals are common in domestic farms.

@fill_in_all_blank[
question.image = http://.../a_landscape_image.png
]
Sky is_____ and plants have______ color!
*blue
*green
>
The sky is blue and plants are green (at least generally 🙂).

@fill_in_all_blank[
question.image = http://.../a_landscape_image.png
]
Order these faces from the youngest to the oldest
* 
* 
* 
* 
> This question of type "put in order" lets the users drag and reorder answers; useful for practicing steps or chronology. Pictures and sounds are supported.

@fill_in_all_blank[
question.image = http://.../a_landscape_image.png
proposals[0].image = http://.../usa_flag.png
proposals[2].image = http://.../frensh_flag.png
proposals[4].image = http://.../cameroun_flag.png
comments[0].image =http://.../picture_showing_each_county_and_its_capital_plus_flags.png
]
Match country with capital!
*USA
*Washington DC
*France
*Paris
*Cameroon
*Yaoundé
> Cameroon = Yaoundé
USA = Washington DC
France = Paris
```

### A. Define the Question Type Using `@type`
At the beginning of a section, you can define the type of the question using:
Please found bellow the list of supported type

#### ✅ Supported types (from `Qcm.TYPE_*`):
| Type                  | Meaning                              |
|-----------------------|---------------------------------------|
| `auto`               | Auto-detection of type                |
| `single`             | Single choice                         |
| `multiple`           | Multiple choice                       |
| `open`               | Text input (short answer)             |
| `select_all`         | Select multiple per group             |
| `put_in_order`       | Arrange items in correct order        |
| `fill_in_all_blank`  | Fill one text with several blanks     |
| `enumerate_all`      | Enumerate everything globally         |
| `match_all_column`   | Match globally                        |
| `jumbled_word`       | Reconstruct a word                    |
| `jumbled_sentence`   | Reconstruct a sentence                |
| `speech_recognition` | Voice recognition input               |
| `surround_all_right_zone` | Visual zone selection             |

That mean, you can for exemple start your question section with :**@single**, **@open**, **@put_in_order** or any other label from the table above!

---

### B. Add Metadata to the Question
Depending on whether or not you want to add metadata to your quiz you can add or omit the `[]` block entirely.
In case you want to add supported metadata to your question, your anwser proposals or your comment, you should add the `[]` block and put your metadata inside!
For example:
```
@fill_in_all_blank[
question.image = http://.../a_landscape_image.png
proposals[0].image = http://.../usa_flag.png
proposals[2].image = http://.../frensh_flag.png
proposals[4].image = http://.../cameroun_flag.png
comments[0].image =http://.../picture_showing_each_county_and_its_capital_plus_flags.png
]
```
Bellow, we will discuss about supported metadata:

These metadata properties will affect the `Question` from section:
```
question.image = /uri/to/image.png
question.sound = /uri/to/audio.mp3
```
That means you can add image and sound to your questions just by submiting an URL, this url should pont on a downloadable image!
It actually support data-uri (data uri are a kind of uri that embed base64)

Other metadata examples:
```
scoring.success = 1 //Experimental option to spécify a score to apply on success for the specific question
scoring.failure = -0.5 //Experimental option to spécify a score to apply on failure for the specific question
input_help = true //Whether or not the smart input should be turned on for the question
```
These las option will apply to the whole question-and-answer

---

### C. Add Metadata for Each Answer Proposal
Each proposition can have its own metadata, using an index:
```
proposals[0].image = /uri/image0.png
proposals[0].sound = /uri/audio0.mp3
proposals[0].eval_type = equals
proposals[0].case_sensitive = true
proposals[0].clue = Think of oceans
proposals[0].scoring.success = 1
proposals[0].scoring.failure = -0.2
proposals[0].extra[tag] = correct-option
```
Here we have added metadata to the first answer proposal (the answer proposal at index 0), by changing the index, you will be able to apply metadata to question at any index!
For example:
- proposals[1] for the second question
- proposals[3] for the third question 
- proposals[8] for the ninth question 

---

### D. Add Metadata for Each Comment
Same principle with indexed comments:
```
comments[0].image = /comment/image.png
comments[0].sound = /comment/sound.mp3
```
Here we have added metadata to the comment!
Although it looks like the answer-proposals, section, it is important to mention that for now the app only support a single comment section.
Therefore we recommend you to always use the comments[0] to add metadata to your comments

---

### E. Use Markdown or HTML for Styling
You can stylize your content using `$html{}` or `$md{}` syntax:

#### 📘 Example (Markdown)
```
$md{
@single
**Which planet is closest to the sun?**
*Mercury
-Venus
-Earth
> Mercury is the first planet of the solar system.
}
```

#### 📘 Example (HTML)
```
$html{
@open[extras[theme]=space]
<h3>Name a planet of the solar system</h3>
*Earth
*Mars
-Venus
> Earth and Mars are considered habitable.
}
```

---

## 💬 Need help?
Write to us at: [qcmmakerapp@gmail.com](mailto:qcmmakerapp@gmail.com)

Happy quiz making! 🧠✨
