# Penguins2

**Site:** http://mikabr.io/penguins2/

A [datapage](https://github.com/datapages/datapage) for the Redivis dataset [datapages.palmerpenguins](https://stanford.redivis.com/datasets/9g3v-91v2fcg5m?v=1.0) (table `penguins`).

## Updating the site

Every push to `main` rebuilds the site with GitHub Actions and publishes it to GitHub Pages. The main files to edit:

- `_quarto.yml`: the site title, and the Redivis table the site reads (under `redivis:`)
- `_config.yml`: which variables can be plotted, and the plot defaults
- `index.qmd` and `about.qmd`: the homepage and About page (put any images in `images/`)
- `theme.scss`: colors and fonts

The data lives on Redivis. After releasing a new version of the dataset there, rebuild the site by running the "Render and Publish" workflow from the Actions tab.

## Local development

Install [R](https://cloud.r-project.org/) and [Quarto](https://quarto.org/docs/get-started/). Run `renv::restore()` in R to install the R packages, then `quarto preview` to see the site.

---

Made with [Datapage Builder](https://datapages.github.io/datapage-builder/).
