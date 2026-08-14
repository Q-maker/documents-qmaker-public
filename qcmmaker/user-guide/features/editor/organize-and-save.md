# Organize, validate, and save questions

Use the top action bar for quiz-wide editing actions, the right drawer for the question list, and the bottom bar for sequential or numeric navigation.

## Understand validation messages

QcmMaker validates the current page when you move forward or save. The type instruction turns red and states what is missing.

### Selection without a true answer

![Selection validation error](./assets/selection-validation-error.png)

With two or more filled choices, check at least one correct answer. If you intended a typed answer instead, choose the Type answer format explicitly.

### Put in order with too few items

![Put-in-order validation error](./assets/order-validation-error.png)

Enter at least two items in the correct reference order.

Other structured types reject incomplete answer sets: Match columns needs complete pairs, Fill in the blanks needs values for its blanks, and open types need accepted text. Complete or remove an unfinished page before saving it as quiz content.

## Use the action bar

![Save action menu](./assets/actionbar-save-menu.png)

| Control | Purpose |
|---|---|
| Back | Leaves the editor and asks what to do when changes are pending. |
| Save | Saves, saves and plays, or saves and lets you choose a play mode. |
| Delete (X) | Clears or removes the current question. |
| Insert | Duplicates, inserts before/after, pastes, imports, or performs related insertion actions. |
| List | Opens the question drawer. |

## Navigate and reorder with the drawer

![Question drawer](./assets/question-drawer.png)

The right drawer lists every question and highlights the current one.

- Tap the question text to open it.
- Long-press and drag a row to change its position.
- Tap the numbered index at the left of a row to open its popup menu.

![Question index popup menu](./assets/question-index-popup.png)

**Move** explains drag reordering. **Delete** removes that question, so check the selected index before confirming.

## Jump directly to a page

![Fast navigation dialog](./assets/fast-navigation.png)

Tap the page index in the center of the bottom bar, such as `15/16`. Enter a page number and tap **OK**. Use **Previous** and **Next** when reviewing nearby questions, and the index dialog when the destination is farther away.

## Before leaving

1. Resolve any red validation instruction.
2. Save the quiz.
3. Choose **Save & play using** when you need to verify a particular play mode.
4. Check the prompt, answers, media, correction comment, timing, and score as a learner would see them.

Leaving without saving discards the current editing session, including newly attached media.

**Previous:** [Pictures, audio, and comments](media-and-comments.md)

**Next:** [Test the quiz in a play mode](../play-modes/README.md)
