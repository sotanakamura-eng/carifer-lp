# CLAUDE.md

## Project overview

This repository contains the Carifer recruitment landing page for 株式会社TL.
Keep the current editorial visual direction: white, deep navy, thin rules,
large English headings, and a small acid-lime accent.

## Important files

- `app/page.tsx`: page structure and Japanese copy
- `app/globals.css`: all page styling and responsive rules
- `app/layout.tsx`: metadata and document layout
- `public/og.png`: social share image
- `scripts/build-github-pages.mjs`: static GitHub Pages exporter
- `github-pages/index.html`: generated static page; do not hand-edit

## Working rules

1. Preserve the Carifer and 株式会社TL service content unless the user asks to change it.
2. Do not copy source code or copyrighted assets from reference websites.
3. Keep mobile layouts working at widths below 900px and 520px.
4. Keep external consultation links pointed at `https://www.trust-lead.jp/carifer`.
5. After changes, run `npm run build`.
6. If publishing, regenerate `github-pages/index.html` with the exporter and update the root GitHub Pages file.

## Commands

```bash
npm install
npm run dev
npm run build
npm test
```
