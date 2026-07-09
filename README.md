# Personal Website Template

Source for [studiojan.github.io](https://studiojan.github.io), built
with [R Markdown websites](https://rmarkdown.rstudio.com/lesson-13.html) and
deployed automatically by GitHub Actions. Each page currently contains only
its heading — content to be added.

## Structure

| File | Purpose |
| --- | --- |
| `_site.yml` | Site configuration: navbar and shared options |
| `index.Rmd` | Home page (site landing page) |
| `about.Rmd` | About page (bullet links to Home, CV, Profiles, Contact) |
| `cv.Rmd`, `profiles.Rmd`, `contact.Rmd` | About subpages (Profiles holds the ORCID and Google Scholar links) |
| `research.Rmd` | Research page (bullet links to Current, Statistical works, Publications) |
| `current.Rmd`, `statistical-works.Rmd`, `publications.Rmd` | Research subpages |
| `studio.Rmd` | Studio page (bullet links to Blog, Photography, Writing, archived works) |
| `blog.Rmd`, `photography.Rmd`, `writing.Rmd` | Studio subpages |
| `styles.css` | Fonts and colours (Courier, black on white, blue links) |
| `nav-dropdown.html` | Script making the About/Studio dropdowns click through to their pages |

## How to edit

1. Edit the `.Rmd` files (plain Markdown works; R code chunks also work).
2. Commit and push to `main`.
3. GitHub Actions renders the site with `rmarkdown::render_site()` and
   publishes it to GitHub Pages — no local R installation required.

To preview locally instead, install R and RStudio, open
`github_site.Rproj`, and run `rmarkdown::render_site()`; the result appears
in `_site/` (which is git-ignored).
