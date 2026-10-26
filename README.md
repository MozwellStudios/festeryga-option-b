# Festeryga Law, Option B staging

Review-only preview of the Option B design refinement.

- **Staging (Option B):** https://mozwellstudios.github.io/festeryga-option-b/
- **Original (Version A):** https://mozwellstudios.github.io/festeryga-site/ (untouched)
- **Source of truth:** branch [`design-refinement-oct23`](https://github.com/MozwellStudios/festeryga-site/tree/design-refinement-oct23) of `MozwellStudios/festeryga-site`
- **Baseline:** tag `v1.0.0-oct23-baseline` in `festeryga-site`

This repository holds no site files. The workflow in `.github/workflows/deploy.yml` checks out the branch, removes obsolete
comparison pages, enforces `noindex` + `robots.txt Disallow: /`, and publishes to GitHub Pages.

**Update staging:** Actions → "Deploy Option B staging" → Run workflow (or `gh workflow run deploy.yml -R MozwellStudios/festeryga-option-b`).
Pass a tag or commit as `ref` to publish an earlier Option B state.

`noindex` and `robots.txt` keep the preview out of search engines. They are not access protection; anyone with the link can view it.
