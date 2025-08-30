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

QcmMaker allows much more than just basic formatting. Here are all advanced options supported via metadata.

### A. Define the Question Type Using `@type`
At the beginning of a section, you can define the type of the question using:
```
@open
```
Or with metadata:
```
@multiple[
proposal_randomization.type = always
]
```

#### ✅ Supported types (from `Qcm.TYPE_*`):
| Type                  | Meaning                              |
|-----------------------|---------------------------------------|
| `auto`               | Auto-detection of type                |
| `single`             | Single choice                         |
| `multiple`           | Multiple choice                       |
| `open`               | Text input (short answer)             |
| `select_each`        | One selection per group               |
| `put_in_order`       | Arrange items in correct order        |
| `fill_in_each_blank` | Fill multiple blanks                  |
| `enumerate_each`     | Enumerate all correct answers         |
| `match_each_column`  | Match per row                         |

> You can omit the `[]` block entirely if no metadata is used: `@open`

---

### B. Add Metadata to the Question
These properties apply to the `Qcm.getQuestion()` object:
```
question.image = /uri/to/image.png
question.sound = /uri/to/audio.mp3
question.extra[note] = Remember to breathe
```
Other metadata examples:
```
scoring.success = 1
scoring.failure = -0.5
input_help = true
extras[difficulty] = hard
```
These are injected into the Qcm extras via `putExtra(...)`.

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

---

### D. Add Metadata for Each Comment
Same principle with indexed comments:
```
comments[0].image = /comment/image.png
comments[0].sound = /comment/sound.mp3
```

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
