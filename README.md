
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Bayesian Digit Analysis - O’Bayes 2019 (Warwick, UK)

## Overview

This repository accompanies the Bayesian Digit Analysis
[poster](https://github.com/pedro-teles-fonseca/bda-poster-warwick/blob/master/poster.pdf),
presented in the
[O’Bayes 2019](https://warwick.ac.uk/fac/sci/statistics/staff/academic-research/robert/0bayesconference/)
conference in the [University of Warwick](https://warwick.ac.uk) (UK).
The purpose of this repository is to share the data and the code that
were used, facilitating the replicability of obtained results. Some
supplementary graphs and tables are also provided.

<a href="https://github.com/pedro-teles-fonseca/bda-poster-warwick/blob/master/poster.pdf"><img src="https://raw.githubusercontent.com/pedro-teles-fonseca/bayes-digit-analysis-warwick/master/images/poster.png" /></a>

## Instructions

### Prerequisites

In order to run the R scripts provided in this repository, the following
R packages are required:

``` r
library("Hmisc")
library("tidyverse") 
```

It is still possible to reproduce all the results in the poster without
installing any package since `Hmisc` is only used to export R tables in
TeX format and `tidyverse` is only used to produce plots, which are
supplementary material.

### Data

The raw data can be found in the `raw-data.xls` file, stored in the
`data-raw` folder. The reorganized version of the dataset that is
imported by the R scripts is the `data.txt` file, stored in the `data`
folder.

### Reproducibility

We provide a self-contained Rstudio workflow that allows for the
replicability of all the results in the poster. In order to direct R to
the correct working directory you should open `bda-poster-warwick.Rproj`
first. After that, all R scripts stored in the `R` folder should run
smoothly.

### R Scripts

  - `read-data.R` is an auxiliary script that is called within other
    scripts to import the data.

  - `auxiliary-functions.R` contains several functions that we developed
    specifically for Bayesian digit analysis. This script is called
    within other scripts when necessary.

  - The tables in the poster can be reproduced with the
    `poster-tables-bin-beta.R` and `poster-tables-mu-dir.R` scripts.

### Supplementary Materials

  - Plots comparing observed versus expected digit frequencies can be
    found in the `plots` folder. The code that generates the plots can
    be found in the `plots.R` script.

  - The `aux-tables.pdf` file in the `tables-aux` folder is a
    user-friendly compilation of all the tables in the poster. The code
    that generates the results in those tables is in
    `aux-tables-bin.beta.R` and `aux-tables-mu-dir.R`.

## Built With

  - [R](https://www.r-project.org) - Free programming language and
    software environment for statistical computing and graphics.
  - [R Studio](https://www.rstudio.com) - Free and open-source IDE for
    R.
  - [TeX Live](https://www.tug.org/texlive/) - Free distribution of the
    TeX typesetting system.
  - [Texmaker](https://www.xm1math.net/texmaker/) - Cross-platform and
    open-source LaTeX editor.

## Funding

  - [CEMAPRE](https://cemapre.iseg.ulisboa.pt) - Center for Applied
    Mathematics and Economics
  - [FCT](https://www.fct.pt/index.phtml.en) - Foundation for Science
    and Technology (Portugal). Research grant reference:
    SFRH/BD/129918/2017 (funded by the European Social Fund and by
    national funds from the MCTES)

<a href="https://cemapre.iseg.ulisboa.pt"><img src="images/cemapre.png" width="400">
<a href="https://www.fct.pt/index.phtml.en"><img src="images/fct.png" width="190">

## Contacts

  - Author: Pedro Fonseca
    ([ISEG](https://www.iseg.ulisboa.pt/aquila/instituicao/ISEG/)) -
    <pedro.teles.fonseca@outlook.com>

  - Advisor: Prof. Rui Paulo
    ([ISEG](https://www.iseg.ulisboa.pt/aquila/instituicao/ISEG/) and
    [CEMAPRE](https://cemapre.iseg.ulisboa.pt)) - <rui@iseg.ulisboa.pt>
