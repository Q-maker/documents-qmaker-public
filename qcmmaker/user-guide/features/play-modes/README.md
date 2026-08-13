# Play Modes

QcmMaker can launch a quiz in **Exam mode** or **Challenge mode**. You can choose
the mode before playing, and quiz authors can also define which modes a shared
`.qcm` file supports.

Good to know: the two modes are not only visual styles. They create different learning experiences. Exam mode protects the feeling of a real test; Challenge mode helps practice through quick feedback.

| Choose this mode | When you want |
|---|---|
| Exam mode | To simulate an evaluation, manage time across the whole quiz, and see feedback after finishing. |
| Challenge mode | To train quickly, answer under pressure, and learn from immediate feedback. |

## In This Guide

- [Choose a mode](#choose-a-mode-before-playing)
- [Use Exam mode](#exam-mode)
- [Use Challenge mode](#challenge-mode)
- [Set the modes allowed by a quiz](#supported-play-mode)
- [Understand controls, timing, and media](#controls-timing-and-media)
- [Review results, corrections, and replay options](result-and-replay.md)
- [Learn how to answer each question family](exam-question-types/README.md)

## Choose A Mode Before Playing

From the home **Questionnaires** tab, tap the small **Q** icon on a quiz card to
switch between **Exam mode** and **Challenge mode**. The icon is green for Exam
mode and red for Challenge mode.

![Home play mode selector](images/home-play-mode-selector.png)

From a quiz detail page, use the **Game mode** selector before pressing **Play**.

![Detail page](images/previewer-detail.png)

![Play mode selector](images/previewer-play-mode-selector.png)

From the editor, open **Save**, choose **Save & play using**, then select a mode.

![Save and play using](images/save-play-using.png)

Choosing a mode this way controls how the quiz starts for you. It does not
change the modes that the quiz file itself allows.

## Exam Mode

Exam mode works like a test or exam simulator. You can navigate between
questions during the test, use the timer for the whole questionnaire, and review
feedback after finishing.

![Exam mode](images/exam-start.png)

All detailed question-family screenshots use Exam mode as the visual reference.
This keeps empty, filled, correct, incorrect, and partial states consistent.
The same question families can be used in Challenge mode, but navigation rhythm
and the moment when correction appears are different. See
[Exam question types](exam-question-types/README.md).

At the end, QcmMaker shows the score, elapsed time, scoring policy, and actions to replay, correct, or leave.
See [Result and replay](result-and-replay.md) for the actions available after a test.

![Exam result](images/exam-result.png)

## Challenge Mode

Challenge mode is more immediate, like a game against the clock. Questions are
shown one after another, each answer is checked as you play, and QcmMaker can
move automatically to the next question depending on the quiz and player
settings.

![Challenge mode](images/challenge-start.png)

Challenge uses the same question families documented in the Exam visual guide.
The important difference is timing: an answer is checked during the run, a
success, failure, partial, or skipped message may appear, and the player then
moves on automatically or waits for your action according to its settings.

The result dialog keeps the same core actions: replay, correct, or leave. See
[Result and replay](result-and-replay.md) for the result dialog and replay
choices.

![Challenge result](images/challenge-result.png)

## Supported Play Mode

When editing a quiz, the **Supported play mode** setting defines which modes the
exported `.qcm` file can use. Open the quiz information editor, then change the
**Supported play mode** row.

![Editor supported play mode](images/editor-supported-play-mode.png)

The available values are:

- **auto**: lets QcmMaker use the quiz and app default behaviour.
- **Challenge only**: the quiz can only be played in Challenge mode.
- **Exam only**: the quiz can only be played in Exam mode.
- **Exam & Challenge**: both modes are allowed, with Exam mode proposed first
  when the player has not explicitly chosen a mode.
- **Challenge & Exam**: both modes are allowed, with Challenge mode proposed
  first when the player has not explicitly chosen a mode.

This setting belongs to the quiz authoring configuration. It is different from
the play-mode selector shown on the home and detail pages, which only selects
the mode for the current play session.

What happens when you share the quiz: the supported play mode setting travels with the exported `.qcm` file. It tells other compatible readers which experience the author intended to allow.

## Controls, Timing, And Media

- Exam mode provides Previous and Next navigation and a question/status drawer,
  so you can revisit answers before finishing. You can also swipe left or right
  between questions. The drawer reports pages, answered questions, remaining
  questions, questions seen, and remaining time, and includes a **Finish the
  test** action. The last Next action also becomes the finish action.
- Challenge mode normally progresses sequentially. During immediate feedback,
  its next-question countdown can be automatic or require your action, depending
  on the quiz and player settings.
- In Challenge mode, the header can show points earned and the current
  question's remaining time. Composed answers expose **Reset** and **Submit**;
  after submission, the feedback area can show an explanation with its own
  picture or sound, a success/failure message, a bookmark action, **Pause**, and
  **Next**.
- A quiz can use a global time limit, a per-question countdown, or no visible
  limit. Pause availability and timer display depend on the selected mode and
  configuration.
- Questions and proposals can include pictures and sounds. Tap the visible media
  controls to enlarge a picture or play audio when they are available.
- Pressing Android Back while a run is active asks for confirmation before
  leaving and explicitly warns that current progress will be lost. In
  correction, navigation returns through the review flow.
- QcmMaker preserves the active run when Android recreates the screen whenever
  the saved quiz and session state remain available. After a rotation or an
  interruption, check the restored question and timer before continuing.

Accessibility depends partly on the content authored in the quiz. Prefer clear
question text, meaningful media, and sufficiently short answers; use the system
keyboard for text fields and the labeled player buttons for navigation. Some
image-only actions may not provide a useful spoken label, so users relying on a
screen reader may need assistance with media-only controls.

## Results, Correction, And Replay

Correction availability depends on the quiz configuration. An author can allow
full or limited correction, or prevent correction entirely. When it is
available, the correction view lets you revisit answers and reopen the score.

See [Result and replay](result-and-replay.md) for the result actions, correction
drawer, and focused replay choices.
