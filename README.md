# rohitkharanghar.github.io

Personal site: https://rohitkharanghar.github.io

Sections:

- **Home** (`index.html`): intro page.
- **Engineering blogs** (`engineering/index.html`): lists posts from `_engineering_posts/`.
- **Notes on Living: Nichijō** (`notes-on-living/index.html`): lists essays from `_posts/`.
- **Interests & reading** (`interests/index.html`): edit the HTML directly.

## Add an essay

Create `_posts/YYYY-MM-DD-title.md`. The date comes from the filename.

```
---
title: On waiting for buses
---

First paragraph is the short intro shown on the list.

The rest of the essay goes here.
```

## Add an engineering post

Create `_engineering_posts/title.md`. Don't put a date in the filename. Set the date in the front matter instead.

```
---
title: Why our retries use jitter
date: 2026-11-20
---

First paragraph is the short intro shown on the list.

The rest of the post goes here.
```

## Publish

```
git add -A
git commit -m "Add post: <title>"
git push
```

GitHub Pages rebuilds in about 1–2 minutes. Check the **Actions** tab for "pages build and deployment".

## Preview locally

```
export PATH="/opt/homebrew/lib/ruby/gems/4.0.0/bin:/opt/homebrew/opt/ruby/bin:$PATH"
jekyll serve
```

Open http://localhost:4000.

## Notes

- Use quotes around titles that contain `:`.
- Jekyll is pinned to nothing; GitHub Pages builds the site with its own version.
