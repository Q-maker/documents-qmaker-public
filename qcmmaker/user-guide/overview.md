# QcmMaker — Product Overview

**App:** QcmMaker (Android)
**Product family:** QmakerTech / Qmaker-algorithm

## What It Does

QcmMaker is a quiz authoring and practice app for Android. An author creates a quiz
file (`.qcm`) containing questions of various types, then plays it locally, shares it
with learners, or imports/exports it across devices. The app is available in several editions (QcmMaker, QcmMaker Plus, QcmMaker Pro)
with different feature sets; all editions are referred to as "QcmMaker" in this guide.

## Getting Started

| Guide | Description |
|---|---|
| [Interface overview](getting-started/interface-overview.md) | Home screen areas, quiz card options, selection mode |
| [Workspace setup](getting-started/workspace-setup.md) | Grant folder permission, choose a working directory |
| [Creating your first quiz](getting-started/first-quiz.md) | End-to-end walkthrough for new users |

## Feature Summary

| Feature | What it does | Detailed doc |
|---|---|---|
| **Create a quiz** | Create a `.qcm` quiz file and add questions (selection, open answer, put-in-order, enumeration, match-column, fill-in-blanks, jumbled words). Attach images and audio to questions and propositions. | [features/create-quiz/](features/create-quiz/README.md) |
| **Search** | Filter the home quiz list by name or keyword. | [features/search/](features/search/README.md) |
| **Play modes** | Play a quiz in **Exam** mode (timed, feedback at end) or **Challenge** mode (immediate per-question feedback). Choose a mode before playing, configure which modes a quiz supports, review correction and score after completion, use the [Exam question type reference](features/play-modes/exam-question-types/README.md) or [Challenge question type reference](features/play-modes/challenge-question-types/README.md) to preview captured question families, and see [Result and replay](features/play-modes/result-and-replay.md) for retake options after a test. | [features/play-modes/](features/play-modes/README.md) |
| **Import & Export** | Import questions from an existing `.qcm` file or from a prepared text Q&A file. Start with the [standard TXT format](features/import-export/import-txt-standard.md), then use the advanced format when you need question types, media, or metadata. Export and share `.qcm` files via Android share sheet. | [features/import-export/](features/import-export/README.md) |
| **Sharing** | Share a `.qcm` file through Android's share sheet. Recipients can open quiz links directly in QcmMaker via Android App Links. | [features/sharing/](features/sharing/README.md) |
| **Bookmarks** | Save specific questions into system or custom bookmark groups, then review or replay those focused question sets later. | [features/bookmarks/](features/bookmarks/README.md) |
| **Settings** | Configure quiz player behaviour (show correct answer, randomise questions, timer…) and app language. | [features/settings/](features/settings/README.md) |
| **Premium features** | Unlock ad-free usage and additional features via an activation code or in-app purchase. | [features/premium/](features/premium/README.md) |
| **About and contact** | View app version, send feedback, share the app. | [features/about/](features/about/README.md) |

## File Formats

`.qcm` is the native binary quiz format. Plain-text import formats (`.txt`) are
also supported. See [file-formats/](file-formats/) for format specifications.
