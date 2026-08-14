# Edit questions

> Lire cette page en [français](README-fr.md).

**Goal:** create valid questions, define the expected answers, and organize them into a quiz.

**Starting point:** open a quiz and tap **EDIT QUESTIONS**. Each editor page represents one question.

The question editor brings together the prompt, answer logic, optional media, a correction explanation, and navigation between questions.

## Create a question in four steps

![Completed selection question from the English Demo quiz](./assets/selection-filled.png)

1. Enter the question in the large field at the top.
2. Tap the type icon in the answer card and choose how the learner must answer.
3. Fill the answer section according to the instruction shown above it.
4. Tap **Next** or **Save**. If the page is incomplete, the instruction turns red and explains what is missing.

## Understand the screen

| Area | Purpose |
|---|---|
| Top action bar | Leave, save/play, clear, insert, duplicate, import, or open the question list. |
| Question header | Enter the prompt and attach a picture or audio. |
| Type instruction | Explains what the active type expects and displays validation errors. |
| Answer card header | Opens quick entries, the type selector, and type-specific advanced options. |
| Answer section | Edits choices, accepted answers, ordered items, blanks, or pairs. |
| Comment section | Adds an explanation shown during correction. |
| Bottom bar | Moves to the previous/next question or opens fast navigation from the center index. |

## Choose the right type

| Type | The learner… | Editor structure |
|---|---|---|
| [Selection](question-types/selection.md) | selects one or more choices | Full-width answer list with correctness controls |
| [Type answer](question-types/typed-answer.md) | types a free answer | Full-width list of accepted answers |
| [Enumeration](question-types/enumeration.md) | provides several expected items | Full-width list of expected items |
| [Fill in the blanks](question-types/fill-in-blanks.md) | completes missing parts | Full-width list of blank values and optional clues |
| [Match columns](question-types/match-columns.md) | matches left and right items | **Two-column grid of paired cells** |
| [Put in order](question-types/put-in-order.md) | restores the reference order | Reorderable full-width list |
| [Jumbled words](question-types/jumbled-words.md) | reconstructs a sentence | Ordered words or fragments |

See the [question type comparison](question-types/README.md) when you are unsure which format to use.

## Empty and completed answer sections

<p align="center">
  <img src="./assets/selection-empty.png" alt="Empty selection answer section with one blank row" width="360" />
  <img src="./assets/selection-filled.png" alt="Completed selection question with checked correct answers" width="360" />
</p>

An empty selection page starts with one answer row. Fill it, use **Add an answer** to add choices, then check every correct answer. The handle on the left moves a row and **X** removes it.

The meaning of a row changes with the type: it can be a choice, an accepted text, an expected item, one side of a pair, or one item in a reference order. Follow the instruction above the card rather than applying selection rules to every type.

## Go directly to a task

- [Understand every question type](question-types/README.md)
- [Use type-specific question and answer options](answer-options.md)
- [Add pictures, audio, and correction comments](media-and-comments.md)
- [Fix validation errors, reorder, navigate, and save](organize-and-save.md)

**Previous:** [Edit quiz information](../create-quiz/edit-information.md)

**Next:** [Choose a question type](question-types/README.md)
