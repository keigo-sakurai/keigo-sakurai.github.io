# keigo-sakurai.github.io

Personal academic website of **Keigo Sakurai** — Assistant Professor at Hokkaido University.

Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme. Deployed via GitHub Pages.

## How to update

- **Bio / top page**: `_pages/about.md` (EN), `_pages/about_ja.md` (JA)
- **Publications**: `_bibliography/papers.bib` (BibTeX; `selected = {true}` shows a paper on the top page)
- **News**: add a Markdown file under `_news/`
- **CV**: `_data/cv.yml`
- **Profile photo**: replace `assets/img/prof_pic.jpg`
- **Social links**: `_data/socials.yml`

Pushing to `main` triggers the GitHub Actions workflow (`.github/workflows/deploy.yml`), which builds the site and publishes it to the `gh-pages` branch.

## Local preview

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000/
```
