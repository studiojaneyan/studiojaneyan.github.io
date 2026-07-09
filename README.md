# Personal Website Template

Source for [studiojan.github.io](https://studiojan.github.io), built
with [R Markdown websites](https://rmarkdown.rstudio.com/lesson-13.html) and
deployed automatically by GitHub Actions. Each page currently contains only
its heading — content to be added.

## Structure

| File | Purpose |
| --- | --- |
| `_site.yml` | Site configuration: navbar and shared options |
| `index.Rmd` | About page (site landing page) |
| `publications.Rmd` | Publications page |
| `profiles.Rmd` | Profiles page (profile links) |
| `styles.css` | Fonts and colours (Courier, black on white, blue links) |

## How to edit

1. Edit the `.Rmd` files (plain Markdown works; R code chunks also work).
2. Commit and push to `main`.
3. GitHub Actions renders the site with `rmarkdown::render_site()` and
   publishes it to GitHub Pages — no local R installation required.

To preview locally instead, install R and RStudio, open
`github_site.Rproj`, and run `rmarkdown::render_site()`; the result appears
in `_site/` (which is git-ignored).
