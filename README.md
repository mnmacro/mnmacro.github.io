# Minnesota Workshop in Macroeconomic Theory

GitHub Pages site for the Minnesota Workshop in Macroeconomic Theory. Content was migrated from the original Google Sites version at
`https://sites.google.com/umn.edu/minnesotamacroworkshop`.

## Local development

```
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000>.

## Deployment

GitHub Pages will build the site automatically from the `main` branch (Settings → Pages → Source: `main` / root). The site is served at <https://mnmacro.github.io>.

## Structure

- `_config.yml` — site metadata and the `past_years` list that drives the nav and Home page
- `_layouts/` — `default.html` (shell) and `past.html` (per-year program template)
- `_includes/nav.html` — top nav with a Past-years dropdown
- `assets/css/style.css` — styling (UMN maroon + gold)
- `index.md` — Home page
- `past/<year>.md` — one file per past conference; front matter sets `title`, `dates`, `location`, `organizers`

## Adding a new year

1. Create `past/<year>.md` using an existing year as a template.
2. Prepend the new year to the `past_years:` list in `_config.yml` so it appears at the top of the nav and Home page.
