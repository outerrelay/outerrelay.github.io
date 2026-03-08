# Economic Security Notes — GitHub Pages + Jekyll starter

A clean, research-oriented starter blog for GitHub Pages.

## What is included

- Home page with featured intro and recent posts
- About page
- Categories index
- Individual category landing pages
- Post template
- Clean white design with black / gray / muted purple accents

## Quick start on GitHub Pages

1. Create a repository named `username.github.io` (or any repo if you prefer project pages).
2. Upload all files from this folder.
3. In GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and the root folder.
6. Save. GitHub Pages will build the site automatically.

## Local preview

If you want to preview locally:

```bash
bundle install
bundle exec jekyll serve
```

Then open the local address shown in the terminal.

## Customize

Edit these first:

- `_config.yml` → site title and description
- `about.md` → your biography and focus areas
- `index.md` → homepage intro text
- `_posts/` → your posts
- `assets/css/style.scss` → colors and styling

## Suggested first categories

- trade-dependencies
- reverse-dependencies
- energy-security
- economic-security
- methods-data

## Writing workflow

1. Duplicate `_draft-post-template.md`
2. Rename it to `YYYY-MM-DD-title.md`
3. Fill in title, excerpt, categories, and content
4. Commit and push

