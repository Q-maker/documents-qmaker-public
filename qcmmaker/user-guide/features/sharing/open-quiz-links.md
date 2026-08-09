# Share and Open Hosted Quiz Links

An HTTP link is an address pointing to a quiz or QcmMaker resource hosted at a remote location. The link is not the `.qcm` file itself: it tells QcmMaker or the web reader where to find the hosted content.

Link sharing is an additional option for people whose `.qcm` files are already hosted online, or who want to host them so that recipients can access the remote quiz through an address.

## When to Share a Link

Use a hosted link when:

- the `.qcm` file or compatible quiz resource is available from an online location;
- you prefer to distribute an address instead of attaching a copy of the file;
- recipients should tap an address that opens a preview, quiz, or exam mode;
- you accept that access depends on the remote location remaining available.

Unlike native `.qcm` file sharing, a link does not by itself give the receiver a standalone local copy. Opening remote content normally requires a network connection and continued access to the hosting location.

## How Compatible Links Open

QcmMaker can open supported QcmMaker and QcmFile links directly from Android. When QcmMaker is installed, tapping a compatible link can open the quiz, exam, project, or documentation inside the app. When the app is not installed, the web reader can handle supported quiz links.

Some Android devices may ask which app should open the link the first time. Choose QcmMaker to continue in the app.

## Supported Links

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

The `src` value is the remote address of the quiz, project, or document to open. It should be URL encoded when it contains special characters.

## Examples

Open a hosted quiz in preview mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F
```

Start the same hosted quiz in quiz mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=quiz
```

Start the same hosted quiz in exam mode:

```text
https://read.qcmfile.com/open?src=https%3A%2F%2Fexample.com%2Fdemo%2F&mode=exam
```

Open a documentation page:

```text
https://doc.qcmmaker.com/documentations/play-modes/body.md
```

## Access and Local Copies

Remote content remains dependent on its hosting location. If that location becomes unavailable, restricted, moved, or deleted, the link may stop working.

When QcmMaker lets you save or import a remote quiz into your workspace, the saved occurrence becomes a local copy. Changes made to that local copy do not modify the hosted source unless you separately control and update the remote location.

## Prefer Native File Sharing?

If you want the receiver to obtain the `.qcm` file itself, keep a local copy, and use it without depending on the original hosting address, see [Share a quiz as a `.qcm` file](share-a-qcm-file.md).
