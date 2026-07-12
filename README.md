# arlendean.com — personal academic website

Personal website of Arlen Dean, built with [Jekyll](https://jekyllrb.com/) and the
[al-folio](https://github.com/alshedivat/al-folio) theme (MIT licensed, see `LICENSE`).

## Editing content

| What | Where |
| --- | --- |
| Home page bio | `_pages/about.md` |
| Publications / papers under review / working papers | `_data/publications.yml`, `_data/submittedpapers.yml`, `_data/workingpapers.yml` |
| CV | `_data/cv.yml` |
| Teaching | `_pages/teaching.md` |
| Talks (page hidden from nav) | `_pages/talks.md` + `_bibliography/talks.bib` |
| News items (currently hidden on home page) | `_news/` |
| Site settings (name, email, URL, nav, colors on/off) | `_config.yml` |
| Colors & fonts | `_sass/_variables.scss`, `_sass/_themes.scss` |

## Running locally

With Docker (recommended, no Ruby setup needed):

```bash
docker compose up
```

then open <http://localhost:8080>.

Or with a local Ruby toolchain:

```bash
bundle install
bundle exec jekyll serve
```

## Deploying

Build the static site with `bundle exec jekyll build` (output in `_site/`) and upload
it to the web host. Do not commit the generated `_site/` output — or any built
HTML — back into this repository.
