# Decomposing the drivers of Bd persistence

**Contributors**: Jake E. and Mark W.

## Objectives

We want a pipeline where we can feed in seasonal prevalence, intensity, and abundance data and get time-varying outputs of these quantities with uncertainty. We will then combine these estimates using a model like Fenton et al. 2015, Bielby et al. 2021, or Wilber et al. 2022 to estimate relative species contributions to Bd persistence.

## Systems of interest

1.  Pennsylvania
    -   This will definitely work with PA data. Michel O. has already done a lot of GAM analyses on the PA SERDP data and we should get in touch with her so you can look at her code.
2.  Brazil
    -   Not sure how amenable the Brazil data will be to these analyses

## Data inputs

1.  Seasonal amphibian abundance data
2.  Seasonal Bd prevalence data
3.  Seasonal Bd infection intensity data
4.  Seasonal habitat use data
    -   Ignore this one for now. We will need to think through the data a bit more.

## Outputs

1.  Species-specific estimates of abundance (with error) through time

    -   Using n-mixture models or mark-recapture methods

2.  Time-varying, species-specific seasonal estimates of prevalence data

    -   Use general additive models (GAMs)

    -   Mean estimates and uncertainty for each species

    -   Try pooling data across years to get a 1-year curve informed by multiple years of data

    -   Alternatively, try estimating GAM across multiple years

3.  Time-varying, species-specific seasonal estimates of Bd infection intensity

    -   Use general additive models (GAMs)

    -   Mean estimates and uncertainty for each species

    -   As with prevalence, try pooling across years and/or estimating curve across multiple years
