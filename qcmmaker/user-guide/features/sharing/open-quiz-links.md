# Open Shared Quiz Links

QcmMaker can open supported QcmMaker and QcmFile links directly from Android. When QcmMaker is installed, tapping one of these links can open the quiz, exam, project, or documentation inside the app. When the app is not installed, the same link can still be handled by the web reader when the website supports it.

The web reader also has a separate local-file workflow: visit [read.qcmfile.com](https://read.qcmfile.com) and select a `.qcm` file from your device. Opening a local file this way does not require you to create or host a remote link.

## Supported Links

Use these links when sharing content with another QcmMaker user:

Good to know: a web link points to a remote quiz or document location. Hosting is needed when you want to give other people a remote link, but not when you only want to select and read a local `.qcm` file in the web reader.

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

What happens next: once the quiz is in your own workspace, edits belong to your local copy. The original remote file is not changed unless you control the place where it is hosted.

If you received a file instead of a link, see [Read a shared `.qcm` file](read-a-shared-qcm-file.md).
