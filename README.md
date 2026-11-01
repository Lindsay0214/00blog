# Personal Blog — Astro

A personal blog and portfolio experiment built with **Astro, MDX, and Tailwind CSS**, based on the Dante theme by [Just Good UI](https://justgoodui.com/).

## Repository contents

- Blog and project content collections.
- Tag pages and pagination.
- RSS and sitemap integration.
- Shared layouts, navigation, and a theme toggle.
- Site configuration and Markdown/MDX content.

The theme provides much of the site's structure and UI. These features should not be interpreted as independently designed implementations by the repository owner.

## Start here

| Path | Purpose |
| --- | --- |
| `src/data/site-config.ts` | Site identity and navigation |
| `src/content/blog/` | Blog content |
| `src/content/projects/` | Project descriptions |
| `src/content/pages/` | About and other static pages |
| `src/pages/` | Astro routes |
| `src/components/` | Shared UI components |

## Run locally

```sh
npm install
npm run dev
```

Use the local URL printed by Astro.

```sh
npm run build
npm run preview
```

## Current status

This repository is a content-site experiment rather than a flagship engineering case study. Some content remains demonstration material: the code-review article explicitly credits AI-assisted demo content, and the beverage project page contains an unrelated sustainability introduction that needs editorial correction.

Before presenting the site as a portfolio, review every project description, replace demonstration content with original case studies, and verify the deployed site and links.
