## Alexandr Wolodarkij — Indie game dev site

This repo powers octobernight.games, a Jekyll site built on the `jekyll-theme-minimal` theme with a custom layer of SCSS.

### Structure

- `index.md` – quick intro, current obsessions, featured builds, contact link
- `about.md` – artist statement plus current experiments
- `projects.md` – renders `_projects/` collection with detailed write-ups
- `blog.md` – dev log index listing posts in `_posts/`
- `_projects/` – markdown files describing each game experiment
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
