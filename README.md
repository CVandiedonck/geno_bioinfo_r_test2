# Objective

This repository contains the practical material to use on PlasmaBio for the fisrst session of my R lectures to the master students of the magistère européen de génétique at Université de Paris.

There is a preparatory session followed by 7 sessions:

- R0: 1st steps with R
- R1: R environment, main R objetcs and particularly vectors.
- R2: TBA
- R3: TBA
- R4: TBA
- R5: TBA
- R6: TBA
- R7: TBA

## Try it on Binder

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/plasmabio/template-r/master?urlpath=%2Flab/)


## Structure of the repo

This repository is based on the [binder-examples/conda](https://github.com/binder-examples/conda) example.

[`repo2docker`](https://repo2docker.readthedocs.io) is the underlying tool that is used to build an environment from a repository.

`repo2docker` can be configured with several types of files. In the case of this repo:

- `binder/environment.yml`: specify dependencies that will be installed using `conda`
- `binder/postBuild`: specify extra dependencies:
  - JupyterLab extensions,
  - R or Bioconductor packages *not available* in [Anaconda cloud](https://anaconda.org/) (*i.e* not installable by `conda`).

Both Jupyter Lab and RStudio are installed.

Once created, the environment can be reused without building it again.

For more information, see the [extensive rep2docker documentation](https://repo2docker.readthedocs.io).


## Materials

Materials can be added anywhere to this repository, either at the top level or in subdirectory.

When building the environment, the materials (and any other file) will be copied to the Docker image.
