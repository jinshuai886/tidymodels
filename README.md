<img src="tidymodels_hex.png" align="center" height = "80px" align = "middle"/>

[![R build status](https://github.com/tidymodels/tidymodels/workflows/R-CMD-check/badge.svg)](https://github.com/tidymodels/tidymodels)
[![Coverage status](https://codecov.io/gh/tidymodels/tidymodels/branch/master/graph/badge.svg)](https://codecov.io/github/tidymodels/tidymodels?branch=master)
[![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/tidymodels)](http://cran.r-project.org/web/packages/tidymodels)
[![Downloads](http://cranlogs.r-pkg.org/badges/tidymodels)](http://cran.rstudio.com/package=tidymodels)
![](https://img.shields.io/badge/lifecycle-experimental-orange.svg)


`tidymodels` is a "meta-package" for modeling and statistical analysis that share the underlying design philosophy, grammar, and data structures of the tidyverse.

It includes a core set of packages that are loaded on startup:

* [`broom`](https://broom.tidyverse.org/) takes the messy output of built-in functions in R, such as `lm`, `nls`, or `t.test`, and turns them into tidy data frames.

* [`dials`](https://tidymodels.github.io/dials/) has tools to create and manage values of tuning parameters.

* [`dplyr`](http://dplyr.tidyverse.org) contains a grammar for data manipulation. 

* [`ggplot2`](http://ggplot2.tidyverse.org) implements a grammar of graphics. 

* [`infer`](http://infer.netlify.com/) is a modern approach to statistical inference.

* [`parsnip`](https://tidymodels.github.io/parsnip/) is a tidy, unified interface to creating models. 

* [`purrr`](http://purrr.tidyverse.org) is a functional programming toolkit.

* [`recipes`](https://tidymodels.github.io/recipes/) is a general data preprocessor with a modern interface. It can create model matrices that incorporate feature engineering, imputation, and other help tools.

* [`rsample`](https://tidymodels.github.io/rsample/) has infrastructure for _resampling_ data so that models can be assessed and empirically validated. 

* [`tibble`](http://tibble.tidyverse.org) has a modern re-imagining of the data frame.

* [`tidyr`](http://tidyr.tidyverse.org) provides tools for reshaping data. 

* [`tune`](https://tidymodels.github.io/tune/) contains the functions to optimize model hyper-parameters.
 
* [`workflows`](https://tidymodels.github.io/workflows/) has methods to combine pre-processing steps and models into a single object. 

* [`yardstick`](https://tidymodels.github.io/yardstick/) contains tools for evaluating models (e.g. accuracy, RMSE, etc.)

There are a few modeling packages that are also installed along with `tidymodels` (but are not attached on startup): 

* [`tidypredict`](https://tidymodels.github.io/tidypredict/) translates some model prediction equations to SQL for high-performance computing.

* [`tidyposterior`](https://tidymodels.github.io/tidyposterior/) can be used to compare models using resampling and Bayesian analysis.

* [`tidytext`](https://github.com/juliasilge/tidytext) contains tidy tools for quantitative text analysis, including basic text summarization, sentiment analysis, and text modeling.


To install:

```r
require(devtools)
devtools::install_github("tidymodels/tidymodels")
```

When loading the package, the versions and conflicts are listed:



```r
library(tidymodels)
```

```
## ── Attaching packages ──────────────────────────────────────────────────────────────────────── tidymodels 0.1.0 ──
```

```
## ✓ broom     0.5.5           ✓ recipes   0.1.10.9000
## ✓ dials     0.0.4.9000      ✓ rsample   0.0.6      
## ✓ dplyr     0.8.5           ✓ tibble    3.0.0      
## ✓ ggplot2   3.3.0           ✓ tune      0.1.0      
## ✓ infer     0.5.1           ✓ workflows 0.1.1.9000 
## ✓ parsnip   0.0.5.9001      ✓ yardstick 0.0.6      
## ✓ purrr     0.3.3
```

```
## ── Conflicts ─────────────────────────────────────────────────────────────────────────── tidymodels_conflicts() ──
## x purrr::discard()  masks scales::discard()
## x dplyr::filter()   masks stats::filter()
## x dplyr::lag()      masks stats::lag()
## x ggplot2::margin() masks dials::margin()
## x recipes::step()   masks stats::step()
```
  
