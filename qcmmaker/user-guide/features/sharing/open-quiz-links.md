# Open Shared Quiz Links

QcmMaker can open supported QcmMaker and QcmFile links directly from Android. When QcmMaker is installed, tapping one of these links can open the quiz, exam, project, or documentation inside the app. When the app is not installed, the same link can still be handled by the web reader when the website supports it.

## Supported Links

Use these links when sharing content with another QcmMaker user:

| Link type | What it opens |
|-----------|---------------|
| `https://read.qcmfile.com/open?src=...` | Quiz preview by default. |
| `https://read.qcmfile.com/open?src=...&mode=quiz` | Quiz player. |
| `https://read.qcmfile.com/open?src=...&mode=exam` | Exam player. |
| `https://preview.qcmfile.com/...` | Quiz preview. |
| `https://quiz.qcmmaker.com/open?src=...` | Quiz player. |
| `https://exam.qcmmaker.com/open?src=...` | Exam player. |
| `https://edit.qcmmaker.com/open?src=...` | Project viewer. |
| `https://doc.qcmmaker.com/...` | QcmMaker documentation. |

The `src` value is the address of the quiz, project, or document to open. It should be URL encoded when it contains special characters.

## Examples

Open a shared quiz in preview mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F
```

Start the same shared quiz in quiz mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=quiz
```

Start the same shared quiz in exam mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=exam
```

Open a documentation page:

```text
https://doc.qcmmaker.com/documentations/play-modes/body.md
```

## Notes

Some Android devices may ask which app should open the link the first time. Choose QcmMaker to continue in the app.

Remote files opened from a link are intended for reading, previewing, or playing. To edit a shared quiz permanently, save or import it into your own workspace first.

