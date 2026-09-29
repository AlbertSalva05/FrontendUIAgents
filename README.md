# Frontend UI Design Agents Collection · v1.3.1

Static site, ready for Render.

## Contents

- `index.html`: the whole site in one self-contained file (styles, scripts, 25 prompts in project order, the 8-phase workflow, and 6 anti-slop files plus the combined summary inlined)
- `assets/logo/`: 4 SVG logo files, used on the design system page and linked for download
- `assets/icons/`: 7 category icons and 14 interface icons (SVG), linked for download
- `render.yaml`: Render Blueprint with security and cache headers
- `robots.txt`

## Deploy on Render

1. Push this folder to its own GitHub or GitLab repository (the files at the repository root).
2. In Render, choose **New > Blueprint** and select the repository. Render reads `render.yaml`.
3. Alternatively choose **New > Static Site**, leave the build command empty and set the publish directory to `.`.

The site uses hash routes (`#/prompts`, `#/workflow`, `#/antislop`, `#/design-system`), so no rewrite rules are needed.

## Updating content

Prompt and anti-slop text is compiled into `index.html`. Edit the source `.md` files in the design project, rebuild, and replace `index.html`.

## Fonts

IBM Plex Sans and IBM Plex Mono, SIL Open Font License 1.1, loaded from Google Fonts.
