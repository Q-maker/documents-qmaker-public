# QcmMaker — Product Overview

**App:** QcmMaker (Android)
**Product family:** QmakerTech / Qmaker-algorithm

## What It Does

QcmMaker is a quiz authoring and practice app for Android. An author creates a quiz
file (`.qcm`) containing questions of various types, then plays it locally, shares it
with learners, or imports/exports it across devices. The app is available in several editions
with different feature sets; all editions are referred to as "QcmMaker" in this guide.

## Key Ideas To Understand First

| Concept | What it means |
|---|---|
| `.qcm` file | The portable quiz document used by QcmMaker. It can contain questions, answers, media, comments, scoring settings, and author information. |
| Workspace | The folder QcmMaker watches and uses to list your quiz files. If a quiz is outside the workspace, you may need to open it manually or add its folder. |
| Quiz project | The quiz you are editing. In the current workspace layout, it is saved as a `.qcm` file that can later be played or shared. |
| Play mode | The experience chosen before starting a quiz. Exam mode waits until the end for feedback; Challenge mode gives quicker feedback while playing. |
| Correction | The review screen shown after a test when the quiz configuration allows it. It helps you understand correct, wrong, missing, or partial answers. |
| Sharing | Sending a portable `.qcm` file or supported quiz link. The receiver needs QcmMaker or another compatible QCM reader to open the file. |
| Author profile | The information used to sign your shared quiz files. If it is empty, a shared file can appear as created by an anonymous author. |
| Import | Adds questions from another `.qcm` quiz or a prepared text file into the quiz you are editing. |
| Premium access | Premium controls advanced tools and access options. It does not remove ownership of quiz files already saved in your workspace. |

## Getting Started

| Guide | Description |
|---|---|
| [Interface overview](getting-started/interface-overview.md) | Home screen areas, quiz card options, selection mode |
| [Workspace setup](getting-started/workspace-setup.md) | Grant folder permission, choose a working directory |
| [Opening an existing `.qcm` file](getting-started/open-qcm-file/README.md) | Open a quiz file from Android's file explorer and add it to the workspace list |
| [Creating your first quiz](getting-started/first-quiz.md) | End-to-end walkthrough for new users |

## Feature Summary

| Feature | What it does | Detailed doc |
|---|---|---|
| **Create a quiz** | Create a `.qcm` quiz file and add questions (selection, open answer, put-in-order, enumeration, match-column, fill-in-blanks, jumbled words). Attach images and audio to questions and propositions. | [features/create-quiz/](features/create-quiz/README.md) |
| **Search** | Filter the home quiz list by name or keyword. | [features/search/](features/search/README.md) |
| **Play modes** | Play a quiz in **Exam** mode (timed, feedback at end) or **Challenge** mode (immediate per-question feedback). Choose a mode before playing, configure which modes a quiz supports, review correction and score after completion, use the [Exam question type reference](features/play-modes/exam-question-types/README.md) or [Challenge question type reference](features/play-modes/challenge-question-types/README.md) to preview captured question families, and see [Result and replay](features/play-modes/result-and-replay.md) for retake options after a test. | [features/play-modes/](features/play-modes/README.md) |
| **Import** | Import questions from an existing `.qcm` file or from a prepared text Q&A file. Start with the [standard TXT format](features/import-export/import-txt-standard.md), then use the advanced format when you need question types, media, or metadata. | [features/import-export/](features/import-export/README.md) |
| **Sharing** | Share a `.qcm` file through Android's share sheet. Recipients can open quiz links directly in QcmMaker via Android App Links. | [features/sharing/](features/sharing/README.md) |
| **Bookmarks** | Save specific questions into system or custom bookmark groups, then review or replay those focused question sets later. | [features/bookmarks/](features/bookmarks/README.md) |
| **Settings** | Configure quiz player behaviour (show correct answer, randomise questions, timer…) and app language. | [features/settings/](features/settings/README.md) |
| **Premium features** | Unlock ad-free usage and additional features via an activation code or in-app purchase. | [features/premium/](features/premium/README.md) |
| **About and contact** | View app version, send feedback, share the app. | [features/about/](features/about/README.md) |

## File Formats

`.qcm` is the native binary quiz format. Plain-text import formats (`.txt`) are
also supported. See [file-formats/](file-formats/) for format specifications.
