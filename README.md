## Alexandr Wolodarkij — Portfolio site

This repository contains the source for Alexandr Wolodarkij’s personal website, built with [Jekyll](https://jekyllrb.com/) and the `jekyll-theme-minimal` theme.

### Structure

- `index.md` – hero landing page highlighting focus areas, projects, testimonials, and contact form
- `about.md` – background, philosophy, and recent engagements
- `projects.md` – collection-driven showcase of project case studies stored in `_projects/`
- `blog.md` – writing hub rendering posts from `_posts/`
- `assets/css/style.scss` – custom styles layered on top of the default theme
- `_layouts/project.html` – tailored layout for long-form project write-ups

### Local development

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000` to preview the site.

### Deployment

The site is compatible with GitHub Pages. Configure repository settings to publish via GitHub Pages with the source set to the default branch.
