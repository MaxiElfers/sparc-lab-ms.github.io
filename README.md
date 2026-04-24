# SPARC Lab website

Source for **https://sparc-lab-ms.github.io/** — the Spatial and Architectural
Cognition (SPARC) Lab at the Institute for Geoinformatics, University of
Münster.

Built with [Hugo](https://gohugo.io/) and the
[Apéro theme](https://hugo-apero.netlify.app/). Deployed via GitHub Actions
to GitHub Pages.

## Adding a news post

News posts live in `content/blog/`. Each post is a folder with an `index.md`
file, so images can sit next to the post.

1. Create a new folder under `content/blog/`, named `YYYY-MM-DD-short-slug/`.
   Example: `content/blog/2026-05-12-new-paper-vr-sketch-maps/`.

2. Inside it, create `index.md` (just copy-paste some old one and modify content)

3. (Required for every news item) Drop a `featured.jpg` into the same folder with a relevant graphic (e.g. key figure of a new paper).

Recommended size: **1000 px on the long edge**, ≤ 300 KB, JPEG for photos,
PNG for diagrams/screenshots. Aspect ratio is flexible (the grid crops),
but landscape ~1000×600 or square 1000×1000 works best.

4. Open a pull request against `main`. Once merged, GitHub Actions builds
   the site and deploys it within a minute or two.

A copyable template is in `content/blog/_example-post/index.md`
(`draft: true`, so it won't appear on the live site).

## Project pages

Template: `content/projects/space-eye/`. Copy that whole folder, rename,
edit the front matter and body. Each project **must** have a card image
named `card.png` — it's what shows on the Projects grid.

- `card.png` — **square, ~1000×1000** (600–1200 px works, keep < 400 KB)
- Supporting figures referenced in the body — any sensible size, keep
  width ≤ 1200 px

Report project publications in APA style with a DOI link, as done on the
SPACE-EYE page.

## Image rules at a glance

| Where | Filename | Size | Required |
|---|---|---|---|
| News post | `featured.jpg` / `.png` | 1000 px long edge | yes |
| Project page | `card.png` | ~1000×1000 square | yes |
| Team portrait | `featured.jpg` | 600×600 square | yes |
| Site-wide | under `static/img/` | see `static/img/README.md` | — |

## Repository layout

```
content/
  _index.md          # home page
  about/             # about section (header/main/sidebar sub-bundles)
  team/              # one folder per person, Apéro list-grid
  publications/      # single long-form page
  teaching and theses/            # open topics + completed theses
  blog/              # news posts
  contact/
static/img/          # favicons, logos, shared images
themes/hugo-apero/   # theme, vendored as a git submodule
hugo.toml            # site config, menus, Apéro params
.github/workflows/
  hugo.yml           # build + deploy to Pages
```

For the Apéro docs: <https://hugo-apero-docs.netlify.app/>.

## One-time setup on GitHub

This repo publishes from the `gh-pages` environment using the Pages GitHub
Action:

## Licence

Content © SPARC Lab. Theme © the Apéro authors (MIT).
