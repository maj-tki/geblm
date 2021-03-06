# geblm: Geometrically Ergodic (Markov Chains for) Bayesian Linear Models

[![Travis build status](https://travis-ci.org/asbates/geblm.svg?branch=master)](https://travis-ci.org/asbates/geblm)
[![Coverage status](https://codecov.io/gh/asbates/geblm/branch/master/graph/badge.svg)](https://codecov.io/github/asbates/geblm?branch=master)

geblm uses geometrically ergodic Gibbs samplers to provide posterior samples for Bayesian linear models and linear mixed models. Using Markov chains that converge at a geometric rate means that a central limit theorem exists and allows for computation of MCMC standard error estimates.

Unlike many MCMC samplers, the algorithms provided in geblm are model specific. This is to ensure geometric ergodicity. Currently the plan is to include support for the following models:

- Linear model with a normal prior.
- Linear mixed model with a flat prior in the fixed effects and a normal prior on the random effects.
- Linear mixed model with a normal prior on the fixed and random effects.
- Linear mixed model with a normal prior on the fixed effects and a *t* prior on the random effects.

This package is primarily meant for students of Stat 676 (Bayesian statistics) 
  at San Diego State University but others may find it useful.


## Installation

geblm is in early development and subject to (possibly substantial) changes. As such, it is not available on [CRAN](https://CRAN.R-project.org). You can install it via the devtools package with:

``` r
devtools::install_github("asbates/geblm")
```



## Background

JC Roman came up with the idea for this package based on his research establishing conditions for geometric ergodicity of Gibbs samplers. The first iteration of this package was developed by JC and Patrick De Jesus. After laying dormant for a while, I started working on it in the fall of 2018. Lo and behold, life happens so this project has become stagnant once again.


