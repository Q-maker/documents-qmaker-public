# Import

QcmMaker can import questions into an existing quiz from another `.qcm` quiz file or from a plain text file.

Import is useful when you already have content somewhere else and do not want to recreate every question manually.

| Source | Best when |
|---|---|
| Existing `.qcm` file | You want to reuse questions from another QcmMaker quiz. |
| Standard TXT file | You want to write simple questions quickly from a phone or computer. |
| Advanced TXT file | You need question types, metadata, media URLs, or styled content. |

From the project information page, open **More options**, then choose **Import questions**.

![Import questions](images/import-questions-dialog.png)

Choose whether the source is a QCM file or a text file.

## Import from a QCM file

For a `.qcm` file, Android opens the file picker. Select the source file to continue the import.

![Import file picker](images/import-qcm-picker.jpg)

What happens next: questions from the selected file are added to the quiz you are editing. The source file remains a separate file.

## Import from a text file

You can also prepare questions and answers in a `.txt` file, including from a computer, then import that file into QcmMaker.

Start with the standard format if you are discovering text import. It is the fastest way to create a ready-to-import file with questions, answers, and optional explanations.

| Need | Recommended guide |
|---|---|
| Create a simple question-and-answer text file quickly | [Standard TXT import](import-txt-standard.md) |
| Add question types, media links, metadata, or styled content | [Advanced TXT import](import-txt-advanced.md) |

Good to know: import changes the quiz you are editing. The source file remains separate, but the imported questions become part of the current quiz.
