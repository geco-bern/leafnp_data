# leafnp data

This contains the leaf Nmass, Pmass, and N:P data, based on Tian et al. (2019) and used for Tian et al. (in prep.)


## Folder `analysis`
Scripts to compile the file containing environmental predictors in addition to just the leaf N and P data are:

- `analysis/01_complement_environment.R` (copied from `leafnp/analysis/leafnp.R` of the `stineb/leafnp` repository).
- `analysis/02_complement_environment_missing.R` (copied from leafnp/analysis/leafnp_complement_missing.R of the `stineb/leafnp` repository)

## Folder `data-raw`

Contains files needed to compile the final file.

## Folder `data`

Contains files produced.

The final file is:

`data/leafnp_tian_et_al.csv`