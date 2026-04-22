# jiayin-resume

Unified workspace for rebuilding Jia-Yin Shih's bilingual resume from the archived 104 export.

## Structure

- `raw/`
  - Immutable source snapshot from 104.
  - `resume-source.html`
  - `resume-source_files/`
- `src/`
  - Editable working files and shared styles for the redesigned resume.
  - `resume.css`
  - `content/`
- Root entry files
  - `index.html` for Chinese
  - `index-en.html` for English
- `assets/`
  - Local reusable assets extracted from the archived snapshot.
  - `images/`
  - `icons/`
  - `docs/`
- `output/`
  - Delivery-ready exports and generated files.

## Rules

- Treat `raw/` as read-only.
- Use `index.html` and `index-en.html` as the outermost entry files.
- Keep shared styles and source copy in `src/`.
- Reuse images from `assets/` instead of linking back to 104 paths.
- Put final exported HTML/PDF in `output/`.
- Keep the root entry files and the exported files aligned.

## Image Inventory

The current `assets/images/` folder already contains renamed local copies of the archived visual assets, including:

- profile cover
- selected project visuals
- portfolio thumbnails
- leadership-related image

## Current Status

- The redesigned bilingual resume is implemented at the workspace root:
  - `index.html`
  - `index-en.html`
- Shared styling lives in `src/resume.css`.
- Export-ready copies live in `output/`:
  - `resume-zh.html`
  - `resume-en.html`
- Archived source materials remain in `raw/`.
