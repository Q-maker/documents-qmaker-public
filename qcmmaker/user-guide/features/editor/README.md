# Editing questions

The question editor is where you write the prompt, choose how the learner must answer, attach media, define accepted answers, add an explanation, and organize the quiz. Each page represents one question.

## How to access

Open a quiz, then tap **Edit questions**.

## Understand the editor

![A completed selection question](./assets/selection-filled.png)

The top area contains the question and its picture/audio controls. The answer card contains three question-level controls: quick entries, question type, and advanced options. Each answer row has its own handle/options area on the left, correctness control when relevant, editable text, and delete button. The bottom bar moves between questions; its center page index opens fast navigation.

## Supported question types

| Type | What the learner does | What you must define |
|---|---|---|
| Selection | Selects one or more answers | Two or more proposals and at least one checked true answer. One filled proposal is treated as a typed answer. |
| Type answer | Types a free answer | One or more accepted answers. |
| Enumeration | Provides several expected items | The expected items and whether all or individual items are evaluated. |
| Fill in the blanks | Completes missing parts of a sentence | The text and expected value for each blank. |
| Match columns | Pairs items from two columns | Complete left/right pairs. |
| Put in order | Restores the correct order | At least two proposals, entered in the correct reference order. |
| Jumbled words | Rearranges words into a sentence | The complete reference sentence. |

Tap the question-type icon in the answer card to change type. The instruction directly above the card updates to state what that type expects.

## Empty and completed answer sections

![An empty answer section](./assets/selection-empty.png)

A new selection question starts with one empty answer row. Enter the question, fill the first proposal, use **Add an answer** for more rows, and check every correct proposal. The left drag handle can reorder proposals; the **X** removes a row.

![A completed answer section](./assets/selection-filled.png)

In a completed selection question, checked boxes are the accepted true answers. Unchecked filled rows remain distractors. For **Put in order**, the displayed authoring order is the reference order; use the row handles or the ordering control to adjust it.

## Question-level advanced options

Tap the vertical three-dot button at the top right of the answer card. The resulting sheet is different for each question-type family:

| Question types | Options shown | Example |
|---|---|---|
| Selection, single/multiple selection | Case sensitivity, input help, answer randomization, and optional display limits | [Selection sheet](./assets/options-sheet-selection.png) |
| Type answer, enumeration | Case sensitivity and input help | [Text-answer sheet](./assets/options-sheet-open-enumeration-panel.png) |
| Fill in the blanks | Case sensitivity | [Fill-blank sheet](./assets/options-sheet-fill-blank.png) |
| Match columns | Randomize the left column, right column, or both | [Match-column sheet](./assets/options-sheet-match-column.png) |
| Put in order, jumbled words | The sheet explicitly reports that this type has no options | [No-options sheet](./assets/options-sheet-no-options.png) |

Types in the same row share the same visual. Randomization is useful for selection questions; Match columns has its own strategy because its two sides can be shuffled independently.

## Options for each answer row

![Answer-row options](./assets/proposition-row-options.png)

Tap the options area on the left of a proposal. Available actions depend on the question type and may include:

- attaching or replacing a picture;
- attaching, recording, generating, listening to, or removing audio;
- choosing how typed text is evaluated: exact equality, contains, or pattern match;
- adding or editing a clue for blank-filling questions;
- reordering the proposal.

Open-ended and enumeration answers do not expose proposition picture/audio actions, while selection, matching, fill-in, and ordering variants can support proposition media.

The visible menu families are:

| Question types | Proposition menu |
|---|---|
| Selection, Match columns, Put in order | Picture and audio submenus. The current Android editor also displays them for Jumbled words, but that type can reject unsupported proposition media during validation. |
| Type answer, Enumeration | Text evaluation only: exact equality, contains, or pattern match. |
| Fill in the blanks | Picture, audio, text evaluation, and clue controls. |

The menu also reacts to the selected proposal. A proposal with an image gains expand/crop/remove commands; one with audio gains listen/remove commands. For Fill in the blanks, an existing clue changes the direct add action into edit/delete choices.

## Question picture and audio

![Question picture menu](./assets/question-picture-menu.png)

The camera button can take a picture, choose one from the device, use a web link, or remove the current image. When an image is already attached, additional layout/crop actions may appear.

![Question audio menu](./assets/question-audio-menu.png)

The audio button can choose an audio file, record sound, use a web link, or create audio from text. Once attached, the player lets you listen and reopen editing options.

## Comment: text, picture, and sound

![Comment editor](./assets/comment-editor.png)

Tap **Add a comment** (or the pencil on an existing comment). A comment is the explanation shown with the question's correction. It can combine text, one picture, and audio. Use **Apply** to keep the changes made in the dialog; the quiz itself still needs to be saved from the editor.

## Validation messages

QcmMaker validates the current question when you move forward or save. The instruction turns red and a short message explains that the page is incomplete.

![Selection validation error](./assets/selection-validation-error.png)

For **Selection**, two or more filled proposals require at least one checked true answer.

![Put-in-order validation error](./assets/order-validation-error.png)

For **Put in order**, enter at least two proposals. Other structured types likewise reject incomplete pairs, blanks, or expected-answer sets; the red instruction states the requirement for the active type. A completely empty trailing page is not a valid question and is ignored or must be completed before it can become quiz content.

## Action bar

![Save menu](./assets/actionbar-save-menu.png)

| Control | Purpose |
|---|---|
| Back | Leaves the editor; if content changed, QcmMaker asks whether to save or discard it. |
| Save | Save, save and play, or save and choose a play mode. |
| Delete (X) | Clears/removes the current question. |
| Insert | Duplicate, insert before/after, paste/import, and related insertion actions. |
| List | Opens the question drawer. |

## Question drawer, reordering, and index menu

![Question drawer](./assets/question-drawer.png)

The right drawer lists every question and highlights the current one. Tap a question's text to jump to it. Long-press and drag a row to reorder questions. Tap the numbered index at the left of a row to open its popup menu; **Move** explains drag reordering and **Delete** removes that question.

![Question index popup menu](./assets/question-index-popup.png)

## Fast navigation

![Fast navigation dialog](./assets/fast-navigation.png)

Tap the page index in the center of the bottom bar (for example, `15/16`), enter a page number, then tap **OK**. This is faster than repeated **Previous**/**Next** taps in a long quiz.

## Before leaving

Use **Save** when the quiz is ready. If a validation message remains, complete the highlighted requirement first. Leaving without saving discards the current editing session, including newly attached media.
