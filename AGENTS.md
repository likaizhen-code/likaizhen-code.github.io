# Repository Guidelines

## Project Structure & Module Organization

This is a Jekyll academic homepage adapted from `luost26/academic-homepage`. Page templates live in `_layouts/` and reusable fragments in `_includes/`. Edit personal details in `_data/profile.yml`, navigation in `_data/navigation.yml`, news in `_news/`, and papers in `_publications/<year>/`. Static CSS, JavaScript, images, and publication covers belong in `assets/`. Jekyll writes the generated site to `_site/`; never edit or commit that directory.

## Build, Test, and Development Commands

- `bundle install --path vendor/bundle` — install the Ruby dependencies locally.
- `bundle exec jekyll serve` — start the development server at `http://127.0.0.1:4000`.
- `bundle exec jekyll build` — generate `_site/` and fail on malformed Liquid or YAML.
- `git diff --check` — catch whitespace errors before committing.

Do not add `.nojekyll`; GitHub Pages must process the Jekyll templates.

## Coding Style & Naming Conventions

Follow the upstream template's four-space indentation in HTML, CSS, JavaScript, YAML, and Liquid. Use snake_case for data fields, kebab-case for CSS classes, and descriptive lowercase filenames such as `_news/2023-joined-shlab.md`. Publication files belong under their publication year and should use `YYYY-short-title.md`.

Keep profile and publication facts in data files instead of hard-coding them into templates. Reuse Bootstrap utilities and existing includes before adding custom CSS or dependencies.

## Testing Guidelines

There is no automated test suite or coverage target. A successful `bundle exec jekyll build` is required. Preview desktop and mobile layouts, then verify navigation, email obfuscation, Scholar/GitHub links, publication covers, and the reduced-motion fallback for the flow-field canvas.

## Commit & Pull Request Guidelines

History uses `Site updated: YYYY-MM-DD HH:MM:SS` for publication snapshots. Focused changes may use concise imperative subjects such as `Update publication metadata`.

Pull requests should summarize content and template changes, list the build command run, and include desktop/mobile screenshots for visual work. Keep generated `_site/`, `vendor/`, and unrelated local files out of commits.

## Security & Content Accuracy

Never commit credentials, private analytics keys, or unpublished personal information. Confirm publication metadata, dates, affiliations, and external URLs before publishing.
