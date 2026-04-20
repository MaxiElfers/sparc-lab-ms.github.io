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
2. Inside it, create `index.md` with this front matter:

   ```yaml
   ---
   title: "Your post title"
   date: 2026-05-12
   author: "Your Name"
   description: "One-sentence summary used on listings and RSS."
   draft: false
   layout: single
   categories:
     - news
   tags:
     - optional-topic
   ---

   Post body in Markdown.
   ```

3. (Optional) Drop a `featured.jpg` into the same folder for a thumbnail.
4. Open a pull request against `main`. Once merged, GitHub Actions builds
   the site and deploys it within a minute or two.

A copyable template is in `content/blog/_example-post/index.md`
(`draft: true`, so it won't appear on the live site).

## Local development

Install the [extended Hugo](https://gohugo.io/installation/) binary (v0.128+),
then:

```bash
git clone --recurse-submodules https://github.com/sparc-lab-ms/sparc-lab-ms.github.io.git
cd sparc-lab-ms.github.io
hugo server -D          # -D includes drafts
```

Open <http://localhost:1313/>. Edit any file under `content/` and the browser
will reload.

If you already cloned without `--recurse-submodules`:

```bash
git submodule update --init --recursive
```

## Repository layout

```
content/
  _index.md          # home page
  about/             # about section (header/main/sidebar sub-bundles)
  team/              # one folder per person, Apéro list-grid
  publications/      # single long-form page
  theses/            # open topics + completed theses
  blog/              # news posts
  contact/
static/img/          # favicons, logos, shared images
themes/hugo-apero/   # theme, vendored as a git submodule
hugo.toml            # site config, menus, Apéro params
.github/workflows/
  hugo.yml           # build + deploy to Pages
```

## Configuration highlights

Edit `hugo.toml` for:

- Site title, `baseURL`, description
- Apéro colour theme (`params.theme`, e.g. `sky`, `plum`, `earth`)
- Fonts (`params.customtextFontFamily`, `params.customheadingFontFamily`)
- Main menu (`[[menu.header]]`) and footer menu (`[[menu.footer]]`)
- Social links (`[[params.social]]`)

For the Apéro docs: <https://hugo-apero-docs.netlify.app/>.

## One-time setup on GitHub

This repo publishes from the `gh-pages` environment using the Pages GitHub
Action:

1. In **Settings → Pages**, set **Source** to **GitHub Actions**.
2. Push to `main` — the `hugo.yml` workflow builds and deploys.
3. The site goes live at <https://sparc-lab-ms.github.io/>.

## Licence

Content © SPARC Lab. Theme © the Apéro authors (MIT).
