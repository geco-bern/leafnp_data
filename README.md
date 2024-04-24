# leafnp_data

This repository contains the leaf Nmass, Pmass, and N:P data, based on Tian et al. (2019), complemented by environmental covariates. The code for complementing the original data by Tian et al. (2019) is contained in this repository and is used for the analysis and modelling for the article Tian et al. (in prep.). Code for the data analysis and modelling is contained in a separate repository [leafnp](https://github.com/stineb/leafnp).

## Workflow

To reproduce the data generation, follow these steps:

1.  Obtain the original data from Tian et al. (2019) (follow link provided therein) and place it locally. In code used here, the file is lives at `data-raw/global_leaf_NP_total_Di_20210224.csv`.
2.  Complement data: `analysis/01_complement_environment.R` (copied from `leafnp/analysis/leafnp.R` of the `stineb/leafnp` repository)
3.  Complement missing environmental data: `analysis/02_complement_environment_missing.R` (copied from leafnp/analysis/leafnp_complement_missing.R of the `stineb/leafnp` repository)

The code relies on the custom R package {ingestr}. Install it from github, available [here](https://github.com/geco-bern/ingestr).

The final file, produced and contained by this rep, is:

`data/leafnp_tian_et_al.csv`

## Repository structure

### Folder `analysis`

Contains scripts (see Workflow above).

### Folder `data-raw`

Contains files needed to compile the final file.

### Folder `data`

Contains files produced by code of this repo (files not contained by this repo).

### Folder `vignettes`

Contains a vignette showcasing the data.

## References

Tian, D., Kattge, J., Chen, Y., Han, W., Luo, Y., He, J., Hu, H., Tang, Z., Ma, S., Yan, Z., Lin, Q., Schmid, B., and Fang, J.: A global database of paired leaf nitrogen and phosphorus concentrations of terrestrial plants, Ecology, 100, e02812, <https://doi.org/10.1002/ecy.2812>, 2019.

Di Tian, Zhengbing Yan, Bernhard Schmid, Jens Kattge, Jingyun Fang, Benjamin D. Stocker: Environmental versus phylogenetic controls on leaf nitrogen and phosphorous concentrations of terrestrial plants. (in review)
