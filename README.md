# Kaizhen Li's Academic Homepage

Personal academic website for [Kaizhen Li](https://likaizhen-code.github.io), built with Jekyll and adapted from [academic-homepage](https://github.com/luost26/academic-homepage).

## Local development

```bash
bundle install --path vendor/bundle
bundle exec jekyll serve
```

Open `http://127.0.0.1:4000`.

## Updating content

- Profile, biography, and education: `_data/profile.yml`
- Navigation: `_data/navigation.yml`
- News: `_news/*.md`
- Publications: `_publications/<year>/*.md`
- Site styling and flow-field visual: `assets/css/global.css` and `assets/js/flow_field.js`

Run `bundle exec jekyll build` before publishing. GitHub Pages builds the site from the repository root.
