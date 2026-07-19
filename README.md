# Introduction to Modern Climate Change

Static GitHub Pages migration of [andrewdessler.com](https://www.andrewdessler.com), the companion site for Andrew Dessler’s textbook *Introduction to Modern Climate Change*.

## What is migrated

- The redesigned public homepage
- The resources directory, with transitional links to all existing chapter pages
- The author biography and links
- Responsive navigation, accessible markup, metadata, and original site imagery
- Automatic deployment through GitHub Actions

The detailed chapter pages, video indexes, exercises, and datasets still link to the Squarespace site so nothing is broken during the migration.

## Run locally

Any static web server will work:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish

The workflow in `.github/workflows/pages.yml` deploys every push to `main`. In the repository settings, choose **GitHub Actions** as the Pages source. The project site will be available at:

`https://aedessler.github.io/intro-modern-climate-change/`

Do not change DNS for `andrewdessler.com` until the remaining content has been migrated and the Pages custom domain has been configured.

## Next migration phase

1. Copy the fourteen chapter resource pages and update their links to local URLs.
2. Migrate the third-edition lecture index, then the archived video pages.
3. Move downloadable exercises and datasets into versioned repository folders.
4. Add a `CNAME` file and update DNS only after a complete content and redirect audit.
