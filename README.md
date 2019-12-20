# testing_travis

[![Build Status](https://travis-ci.com/ismayc/testing_travis.svg?branch=master)](https://travis-ci.com/ismayc/testing_travis)

Automating tests of reproducibility of `.Rmd` files within an RStudio Project using travis-ci. 

## Things to keep in mind

* No explicit activiation of travis-ci required for a GitHub repo if you commit a `.travis.yml` file
* First time running will take a while to install R and packages and cache them. In particular `tidyverse`: approximately 15min.
* Students would be responsible for adding all packages used to TBD: `DESCRIPTION` or `.travis.yml`:
    + CRAN versions under `Imports`
    + GitHub versions under `Remotes`
* `here::here()` takes care of macOS, windows, UNIX variation in file path specifications. 
* The `_build.sh` bash file is set up to test every `.Rmd` file in project folder 
* If students want fancy travis-ci badge above to work, they need to replace `rudeboybert` with their own GitHub login


## TODO

* Record a loom screencast demonstrating all of this
