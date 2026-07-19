# Introduction to Modern Climate Change

Static GitHub Pages companion site for Andrew Dessler’s textbook *Introduction to Modern Climate Change*.

## What is migrated

- The redesigned public homepage
- The resources directory and all fourteen chapter resource pages
- The third-edition, second-edition, and Fall 2012 lecture indexes
- The third-edition data page
- The author biography and links
- Responsive navigation, accessible markup, metadata, and original site imagery
- Automatic deployment through GitHub Actions

Source links from the migrated pages continue to point to their original destinations.

## Run locally

Any static web server will work:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Publish

The workflow in `.github/workflows/pages.yml` deploys every push to `main`. In the repository settings, choose **GitHub Actions** as the Pages source. The project site will be available at:

`https://aedessler.github.io/IMCC-website/`

Do not change DNS for `andrewdessler.com` until the remaining content has been migrated and the Pages custom domain has been configured.

## Next migration phase

1. Move downloadable datasets into versioned repository folders if local copies are desired.
2. Add a `CNAME` file and update DNS only after a complete content and redirect audit.
