# CONTEXT.md — documents-qmaker-public

Public-facing documentation for QmakerTech products.

> **WARNING — Live raw GitHub URLs in production:**
> Several directories in this repository are served directly via raw GitHub URLs
> used by production Android apps. **Do NOT move or rename any of those directories.**
> Only `qcmmaker/user-guide/` (not yet in production) may be relocated.

---

## Directory Map

| Directory | Product | Status | Notes |
|-----------|---------|--------|-------|
| [`documentations/`](./documentations/) | QcmMaker | **LIVE — do not move** | Served via raw GitHub URL in production Android WebViews |
| [`faq/`](./faq/) | QcmMaker | **LIVE — do not move** | Served via raw GitHub URL |
| [`tips/`](./tips/) | QcmMaker | **LIVE — do not move** | Served via raw GitHub URL |
| [`qcmfiles/`](./qcmfiles/) | QcmMaker | **LIVE — do not move** | Sample QCM files |
| [`web/`](./web/) | QcmMaker | **LIVE — do not move** | Web content |
| [`latest-apks/`](./latest-apks/) | QcmMaker | **LIVE — do not move** | APK distribution |
| [`notifications/`](./notifications/) | QcmMaker | **LIVE — do not move** | Operational notification content |
| [`dedal/`](./dedal/) | — | Keep | Marketing / presentation content |
| [`documents/`](./documents/) | — | Keep | Legal documents |
| [`resources/`](./resources/) | Keep | Media and shared assets |
| [`qcmmaker/`](./qcmmaker/CONTEXT.md) | QcmMaker | New canonical dir | `user-guide/` lives here |
| [`qcmkeystore/`](./qcmkeystore/CONTEXT.md) | QcmKeystore | Placeholder | — |
| [`qcmtopdf/`](./qcmtopdf/CONTEXT.md) | QcmToPdf | Placeholder | — |
| [`qcmcopysheetbucket/`](./qcmcopysheetbucket/CONTEXT.md) | CopySheetBucket | Placeholder | — |

---

## Routing Rule

- New user-facing documentation for **QcmMaker** → `qcmmaker/`
- Existing live content under `documentations/`, `faq/`, `tips/` → **MUST stay in place**
- New public docs for other products → create `<product>/` directory here
