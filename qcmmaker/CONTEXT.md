# CONTEXT.md — qcmmaker (documents-qmaker-public)

Public-facing documentation for the **QcmMaker** product.

> **Important:** The main user documentation (`documentations/`) is served via live raw GitHub
> URLs in production Android WebViews. It lives at the **repository root**, not here.
> The `user-guide/` directory here is also live, through the QcmMaker documentation website.

## Public user-guide links — preferred format

For new links shared with users, use the website URLs:

- Guide home: `https://www.qcmmaker.com/user-guide/qcmmaker/`.
- Page: `https://www.qcmmaker.com/user-guide/qcmmaker/getting-started/workspace-setup`.
- `/user-guide/qcmmaker/README` and `/README.md` also open the guide home.

The page path follows the file under `user-guide/`, without `.md`. A trailing directory slash
loads its `README.md`. Keep language suffixes for existing translations, e.g. `README-fr`;
the URL resolver does not choose a language or fall back to another translation automatically.

Prefer these URLs over new `/markdown/?source=https://raw.githubusercontent.com/...` links
in apps, support replies, emails and websites. Existing viewer and GitHub links remain supported.
Inside Markdown sources, keep relative `.md` links and relative media paths: the website resolves
them and converts guide links to the public URL format. Preserve published filenames and paths.

---

## Contents

| Path | Description |
|------|-------------|
| [`user-guide/README.md`](./user-guide/README.md) | User guide index — evergreen intro + TOC + link to overview |
| [`user-guide/overview.md`](./user-guide/overview.md) | Product overview — AI-agent entry point, feature summary with links to sub-pages |
| [`user-guide/faq.md`](./user-guide/faq.md) | User-facing FAQ mined from recurring support questions |
| [`legal/privacy-policy.md`](./legal/privacy-policy.md) | Privacy policy — English. Product-level canonical copy, converted from the legacy `.txt` source. |

## Live Production Documentation

The following directories are at the **repository root** and cannot be moved:

| Path (from repo root) | Description |
|-----------------------|-------------|
| [`../documentations/`](../documentations/) | Full app documentation (WebViews) — **LIVE** |
| [`../faq/`](../faq/) | FAQ — **LIVE** |
| [`../tips/`](../tips/) | Tips & tricks — **LIVE** |
| [`../documents/PrivacyPolicies/en.txt`](../documents/PrivacyPolicies/en.txt) | Legacy privacy policy source — **LIVE / do not move** |

## External Legacy Source

| Path (from workspace root) | Description |
|----------------------------|-------------|
| [`web/qcmmaker/public/documents/PrivacyPolicies/en.txt`](../../web/qcmmaker/public/documents/PrivacyPolicies/en.txt) | Legacy QcmMaker privacy policy source used to create the product-level Markdown copy. |
