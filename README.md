# Writedocs template

Starter for a documentation site built with [Writedocs](https://preview.writedocs.io). The generator (`@writedocs/generator`) is installed **in this project**, pinned in `package.json`, so everyone previewing the docs runs the same version. Nothing needs to be installed globally.

## Use it

1. Create a repo from this template (or copy the folder) and rename it, e.g. `acme-docs`.
2. Install, with [Node.js](https://nodejs.org) 22.12 or newer:

   ```bash
   npm install
   ```

3. Preview:

   ```bash
   npm run dev
   ```

   Opens the site at `http://localhost:4321` and reloads as you edit.

## Scripts

| Script | What it does |
| --- | --- |
| `npm run dev` | Live preview. |
| `npm run validate` | Checks `writedocs.json` and every page, with file and line for each problem. |
| `npm run broken-links` | Finds links that lead nowhere. |
| `npm run check` | `validate` then `broken-links`. Run it before pushing. |

## Layout

```
.
├── package.json        # pins @writedocs/generator
├── writedocs.json      # name, colors, logo, navigation
├── index.mdx           # home page (/)
├── docs/               # pages
├── api-reference/      # API intro + openapi.yaml (endpoint pages are generated)
└── images/             # logos, favicon, page images
```

Every `.md`/`.mdx` file with a frontmatter block in this folder is a page (`node_modules` is skipped). Files without frontmatter, like this README, are ignored. Keep notes or source material that do have frontmatter out of this repo, or they'll show up as pages.

## Make it yours

- `writedocs.json`: change `name`, `description`, `domain`, `styles.colors.primary`, the footer links, and the logo and favicon in `images/`.
- Replace the example pages and `api-reference/openapi.yaml` with your own.
- Delete `docs/writing/` and the "Writing these docs" group when you no longer need them.

## Updating Writedocs

```bash
npm install @writedocs/generator@latest
npm run check
```

Then preview the site before committing the new version.
