# Standard TXT Import

Use the standard TXT format when you want to create questions quickly from a phone or a computer. You write the questions in a normal `.txt` file, save it, then import it into QcmMaker.

This is the recommended format for your first text import because it focuses on the essentials: question, correct answers, wrong answers, and optional explanation.

When to use this: choose the standard format when your quiz is mostly text and you want to prepare many questions faster than entering them one by one in the editor.

## Basic Structure

Each question section contains:

| Part | How to write it |
|---|---|
| Question | Write the question text first. It can use more than one line. |
| Correct answer | Start the answer line with `*`. |
| Wrong answer | Start the answer line with `-`. |
| Explanation | Start the comment line with `>`. This part is optional. |

Example:

```text
Among the following animals,
which of these animals lives in the water?
-Cat
-Dog
*Fish
-Horse
> Fish are aquatic animals.
```

## Add Several Questions

Separate each question section with one blank line.

```text
Among the following animals,
which of these animals lives in the water?
-Cat
-Dog
*Fish
-Horse
> Fish are aquatic animals.

Which of these animals are flying?
*Pigeon
-Dog
*Raven
*Eagle
> Pigeons, ravens, and eagles are birds.
```

## Quick Rules

- Put the question before the answers.
- Use `*` before every correct answer.
- Use `-` before every wrong answer.
- Use `>` before the explanation when you want to add one.
- Leave one empty line between two questions.
- Save the file as `.txt`.
- Prefer UTF-8 encoding, especially if your file contains accents, symbols, or non-English text.

Good to know: the symbols at the start of answer lines tell QcmMaker how to interpret the file. `*` means this answer should be treated as correct, `-` means it is a wrong proposal, and `>` becomes explanation text shown during correction when available.

## Useful Patterns

A question with one correct answer becomes a simple single-answer question.

```text
What is the file extension of a QcmMaker quiz?
*qcm
-docx
-xls
> QcmMaker quizzes are saved as .qcm files.
```

A question with several correct answers can be used for multiple selection.

```text
QcmMaker lets you:
*Create quizzes
*Play quizzes
*Share quizzes
-Edit spreadsheets
> QcmMaker is made for creating, playing, and sharing quiz files.
```

You can start from the sample file here: [demo_standard.txt](../../../../resources/qxt/demo_standard.txt).

When you are comfortable with this structure, you can use [Advanced TXT Import](import-txt-advanced.md) to add question types, media, and metadata.
