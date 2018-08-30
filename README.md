
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![Build Status](https://api.travis-ci.org/dynverse/dynbenchmark.svg)](https://travis-ci.org/dynverse/dynbenchmark) ![Lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg) <a href = "package/man/figures/logo.svg"><img src="package/man/figures/logo.png" align="right" /></a>

# Benchmarking trajectory inference methods

This repo contains the scripts to reproduce the manuscript

A comparison of single-cell trajectory inference methods: towards more accurate and robust tools
Wouter Saelens\*, Robrecht Cannoodt\*, Helena Todorov, Yvan Saeys
bioRxiv 276907; doi: <https://doi.org/10.1101/276907>

## Experiments

From start to finish, the repository is divided into several experiments, each with their own scripts and results. The scripts and results are accompanied by github READMEs and can be easily explored by going to the appropriate folders:

| \#  | id                  | scripts                                                       | results                                                                                                  |
|:----|:--------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------|
| 1   | Datasets            | [Datasets scripts](scripts/01-datasets)                       |                                                                                                          |
| 2   | Metrics             | [Metrics scripts](scripts/02-metrics)                         | [Metrics results](https://github.com/dynverse/dynbenchmark_results/tree/master/02-metrics)               |
| 3   | Methods             | [Methods scripts](scripts/03-methods)                         | [Methods results](https://github.com/dynverse/dynbenchmark_results/tree/master/03-methods)               |
| 4   | Method testing      | [Method testing scripts](scripts/04-method_testing)           | [Method testing results](https://github.com/dynverse/dynbenchmark_results/tree/master/04-method_testing) |
| 5   | Scaling             | [Scaling scripts](scripts/05-scaling)                         | [Scaling results](https://github.com/dynverse/dynbenchmark_results/tree/master/05-scaling)               |
| 6   | Optimise parameters | [Optimise parameters scripts](scripts/06-optimise_parameters) |                                                                                                          |
| 7   | Benchmark           | [Benchmark scripts](scripts/07-benchmark)                     | [Benchmark results](https://github.com/dynverse/dynbenchmark_results/tree/master/07-benchmark)           |
| 8   | Aggregate           | [Aggregate scripts](scripts/08-aggregate)                     |                                                                                                          |
|     | Varia               | [Varia scripts](scripts/varia)                                |                                                                                                          |

We also have several additional subfolders:

-   manuscript: source files for producing the manuscript
-   package: an R package with several helper functions
-   data: raw data files required by the scripts
-   derived: intermediate data files produced by the scripts

## Datasets

The benchmarking pipeline generates (and uses) the following datasets:

-   **Gold standard single-cell datasets**, both real and synthetic, used to evaluated the trajectory inference methods [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1211533.svg)](https://doi.org/10.5281/zenodo.1211533)

![datasets](package/man/figures/datasets.png)

-   **The performance of methods** used in [dynguidelines](https://www.github.com/dynverse/dynguidelines). *Not yet available*

-   **General information about trajectory inference methods**, available as a data frame in `dynmethods::methods`

## Benchmarking your own method

Explanation coming soon. Feel free to make an issue or send us an e-mail if you want your method to be included.

## Guidelines

Based on the results of the benchmark, we provide context-dependent user guidelines. If you want to run methods based on these guidelines, see the [dynorepository](https://github.com/dynverse/dyno). For the guidelines itself, see the [dynguidelines](https://github.com/dynverse/dynguidelines).
