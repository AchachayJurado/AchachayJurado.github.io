# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Natalia Jurado's personal academic/professional website, published as a **GitHub user site** at
https://AchachayJurado.github.io. It is a Jekyll site forked from
[academicpages](https://github.com/academicpages/academicpages.github.io), which itself derives from the
[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme. Most of the repo is inherited theme
machinery (`_includes/`, `_layouts/`, `_sass/`, `assets/js/`); the personal content lives in a handful of
places (see "Where content lives").

## Build, serve, deploy

- **Deployment is automatic.** Pushing to the default branch (`main`) triggers GitHub Pages to build and
  publish the site. There is no manual build/deploy step and no CI config in the repo.
- **No `Gemfile`.** To preview locally you must supply Jekyll yourself, ideally the `github-pages` gem so the
  local build matches production: install it, then `jekyll serve` (or `bundle exec jekyll serve` if you add a
  Gemfile). The site output goes to `_site/` (gitignored).
- **JavaScript bundling** (`package.json`, only needed when editing theme JS):
  - `npm run build:js` — uglifies/concatenates `assets/js/vendor/*`, `assets/js/plugins/*`, and
    `assets/js/_main.js` into `assets/js/main.min.js`. The minified file is committed; regenerate it after
    editing any source JS.
  - `npm run watch:js` — rebuild on change.
- There is **no test suite and no linter.**

## Where content lives

Editing the site almost always means editing Markdown/YAML, not templates:

- `_pages/` — top-level pages. `about.md` (permalink `/`) is the **homepage**; also `cv.md`,
  `publications.md`, `teaching.html`, `year-archive.html`, `404.md`, `sitemap.md`.
- `_publications/*.md` — one file per publication/project (abstracts, papers, demos); rendered via
  `site.publications` on `publications.md` and `cv.md`.
- `_teaching/*.md` — one file per teaching/TA entry; rendered via `site.teaching` on `teaching.html` and
  `cv.md`.
- `_posts/*.md` — blog posts (`YYYY-MM-DD-title.md`), surfaced via `year-archive.html`.
- `_data/navigation.yml` — the top nav bar links.
- `_data/authors.yml`, `_config.yml` (`author:` block) — bio, social links, avatar.
- `images/` — profile photo (`profile_nj.jpeg`), logos.
- `assets/css/main.scss` — the SCSS entry point that pulls in `_sass/`; put custom style overrides here.

Collection items are ordered by `date` in frontmatter and rendered through
`_includes/archive-single.html`. Each item's frontmatter carries `title`, `collection`, `permalink`,
`date`, and (for publications) `venue`/`excerpt`/`paperurl`.

## Collections

`_config.yml` declares collections `publications`, `teaching`, `portfolio`, and `talks`. Jekyll reads each
from the matching `_<name>/` directory, so a content file only appears on the site if it sits in the
directory named after its collection (`_publications/`, `_teaching/`). The `collection:` value in an item's
frontmatter is metadata used by `archive-single.html`; it does **not** by itself place the file in a
collection — the directory does. `portfolio` and `talks` are declared but have no content directories and are
unused.

## Config notes

- Site chrome comes from `_config.yml`: `title`, `name`, `description`, `author:` block, and the `defaults:`
  section that assigns layouts (`single`, `archive`, `talk`) and options (author profile, comments, sharing)
  per content type.
- SCSS is compiled by Jekyll (`sass:` block, `style: compressed`) — do not hand-edit compiled CSS.
- Comments (staticman) and analytics blocks exist in config but are effectively unconfigured/disabled.
