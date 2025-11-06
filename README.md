## Alexandr Wolodarkij — Indie game dev site

This repo powers a Jekyll site built on the `jekyll-theme-minimal` theme with a thin layer of SCSS.

### Structure

- `index.md` – intro, statement excerpt, contact link
- `about.md` – artist statement excerpt
- `projects.md` – placeholder page wired to the `_projects/` collection
- `blog.md` – dev log index (currently empty)
- `_projects/` – collection folder (empty placeholder)
- `assets/css/style.scss` – stylistic overrides for typography, layout, and cards

### Local dev

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` for the live preview.

### Deployment

Ready for GitHub Pages or any static host. Point your domain at the generated `_site` output.
