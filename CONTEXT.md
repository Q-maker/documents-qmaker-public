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

## Public Legal Documents Standard

Every documented public app must expose its legal documents under:

```
<product>/legal/
```

The canonical English privacy policy filename is:

```
<product>/legal/privacy-policy.md
```

Localized variants use a lowercase language suffix:

```
<product>/legal/privacy-policy-fr.md
```

Legacy live files under `documents/PrivacyPolicies/` or other production-served locations must not be
moved or renamed. When a policy already exists there, copy its content into the product-level
`legal/` directory and convert legacy `.txt` sources to properly formatted Markdown.
