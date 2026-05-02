# Implementation Tasks

## Phase 1: Rendering Stability

- [ ] Remove the sample R chunk from `about.qmd`.
- [ ] Confirm `index.qmd` renders as a static page without R package dependencies.
- [x] Remove `index_quarto.qmd` so `index.qmd` is the only homepage source.
- [x] Remove `index_quarto.qmd` from the Quarto navbar.

## Phase 2: Site Structure

- [ ] Replace the About placeholder with lab description, leadership, affiliation, and contact/link information.
- [ ] Convert empty `Research Project Page` links on `index.qmd` into real pages, anchors, or remove the links until targets exist.
- [ ] Create one project-detail page per active research area if separate pages are desired.
- [ ] Update `_quarto.yml` navbar labels so every navigation item has a clear purpose.
- [ ] Confirm the table of contents is useful on each page; disable it on short pages if it adds clutter.

## Phase 3: Content Quality

- [ ] Check source content for character encoding artifacts, especially curly quotes and dashes.
- [ ] Check all institutional names and project titles for consistency.
- [ ] Add a short research status note explaining that reports will be published when complete.
- [ ] Add publication/report placeholders only where there is a clear planned output.

## Phase 4: Visual Design

- [ ] Add baseline styling in `styles.css` for readable page width, project sections, links, and callouts.
- [ ] Keep the design restrained and academic, with enough structure for scanning project summaries.
- [ ] Avoid complex custom SCSS unless the site needs more than Quarto theme customization.
- [ ] Check the rendered site on desktop and narrow viewport widths.

## Phase 5: Build And Deployment

- [ ] Fix local Quarto execution errors for `CMD` and `sass.bat`, or verify the GitHub Actions build succeeds even if local rendering is blocked.
- [ ] Run `quarto render` after source cleanup.
- [ ] Verify `_site/search.json` indexes the current SLGF-Lab content.
- [ ] Confirm GitHub Pages is configured to serve from the publishing target used by the workflow.
- [ ] Push changes to `main` and check the `Quarto Publish` workflow.

## Phase 6: Repository Hygiene

- [ ] Resolve Git safe-directory ownership so normal `git status` works without one-off overrides.
- [x] Ignore generated `_site` files because GitHub Actions publishes generated output.
- [x] Remove `_site` from Git tracking while leaving local files ignored.
- [x] Remove unused generated folders such as `index_files` after choosing `index.qmd` as the only homepage source.
- [x] Ignore common Quarto processing files such as `*_files/`, `*_cache/`, `.knit.md`, and `.utf8.md`.
- [ ] Add a short maintenance note documenting how to render and publish the site.
