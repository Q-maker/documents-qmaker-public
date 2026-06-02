# Advanced TXT Import

Use the advanced TXT format when the standard format is not enough. It lets you declare question types, attach media by URL, add metadata, and use Markdown or HTML content.

Before using this page, make sure you understand [Standard TXT Import](import-txt-standard.md).

## Advanced Question Types

Add a question type at the beginning of a question section with `@type`.

```text
@open
What is the result of (10 + 1) x 2?
*22
> 11 x 2 = 22.
```

Documented type labels include:

| Type | Use it for |
|---|---|
| `auto` | Let QcmMaker detect the question type. |
| `single` | One correct answer. |
| `multiple` | Several correct answers. |
| `open` | Short typed answer. |
| `select_all` | Selection questions with several possible answers. |
| `put_in_order` | Items that must be reordered. |
| `fill_in_all_blank` | Fill several blanks in one text. |
| `enumerate_all` | Enumerate all expected answers. |
| `match_all_column` | Match items across columns. |
| `jumbled_words` | Rebuild a sentence from shuffled words. |

The advanced sample also shows practical variants such as `fill_in_each_blank`, `enumerate_each`, and `match_each_column`.

## Add Metadata

Place metadata inside square brackets after the question type.

```text
@select_all[
question.image = https://example.com/question-picture.png
question.sound = https://example.com/question-audio.mp3
]
Does this sound match this animal?
*Yes
-No
> This is the sound of the animal.
```

The metadata block starts with `[` and ends with `]`. Each metadata line uses this structure:

```text
target.property = value
```

## Add Media to Answers

Use proposal indexes to attach media or options to a specific answer. Indexes start at `0`, so `proposals[0]` is the first answer, `proposals[1]` is the second answer, and so on.

```text
@put_in_order[
proposals[0].image = https://example.com/child.png
proposals[1].image = https://example.com/adult.png
]
Order these faces from youngest to oldest.
*
*
> Drag the answers into the correct order.
```

Common proposal metadata includes:

| Metadata | Purpose |
|---|---|
| `proposals[index].image` | Attach an image to an answer. |
| `proposals[index].sound` | Attach a sound to an answer. |
| `proposals[index].clue` | Add a clue for an answer. |
| `proposals[index].case_sensitive` | Control whether typed answers must match letter case. |

Use downloadable URLs for media. Data URIs may also be used when supported by the app.

## Add Media to Comments

QcmMaker supports one comment section for a question. Use `comments[0]` for comment metadata.

```text
@open[
comments[0].image = https://example.com/explanation.png
]
Quote one color of the rainbow.
*violet
*blue
*green
> The image shows the full rainbow.
```

## Style Content with Markdown or HTML

Wrap a question section in `$md{}` when you want Markdown styling.

```text
$md{
@single
**Which planet is closest to the sun?**
*Mercury
-Venus
-Earth
> Mercury is the first planet of the solar system.
}
```

Wrap a question section in `$html{}` when you need HTML.

```text
$html{
@open
<h3>Name one planet of the solar system</h3>
*Earth
*Mars
> Earth and Mars are planets.
}
```

## Advanced Checklist

- Start with `@type` when you want to force a question type.
- Add `[...]` only when you need metadata.
- Keep proposal indexes aligned with the answer order.
- Use `comments[0]` for comment media.
- Separate question sections with one blank line.
- Prefer UTF-8 encoding.

You can start from the sample file here: [demo_advanced.txt](../../../../resources/qxt/demo_advanced.txt).

For a simpler first import, return to [Standard TXT Import](import-txt-standard.md).
