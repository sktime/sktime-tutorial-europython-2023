![](images/team.jpg)

Welcome to the sktime tutorial at Europython 2023
=================================================

This tutorial is about [sktime] - a unified framework for machine learning with time series. sktime contains algorithms and tools for building, applying, evaluating modular pipelines and composites for a variety of time series learning tasks, including forecasting, classification, regression.

`sktime` is easily extensible by anyone, and interoperable with the pydata/numfocus stack.

This is an introductory `sktime` half-day tutorial with:

* a general introduction to `sktime`
* forecasting with `sktime` - uni/multivariate, hierarchical/global, probabilistic
* feature extraction, transformation pipelines, parameter tuning, autoML
* time series classification, regression, and clustering with `sktime`
* customizing time series distances, kernels, time series aligners and alignment distances
* engineering topics: APIs, estimator and dependency management, writing `sktime` compatible 3rd party estimators
* deploying `sktime` in production using `mlflow` with the `mlflavours` plugin

[sktime]: https://sktime.net

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/sktime-tutorial-europython-2023/main?filepath=notebooks)

## :rocket: How to get started

In the tutorial, we will move through notebooks section by section.

You have different options how to run the tutorial notebooks:

* Run the notebooks in the cloud on [Binder] - for this you don't have to install anything!
* Run the notebooks on your machine. [Clone] this repository, get [conda], install the required packages (`sktime`, `seaborn`, `jupyter`) in an environment, and open the notebooks with that environment. For detail instructions, see below. For troubleshooting, see sktime's more detailed [installation instructions].
* or, use python venv, and/or an editable install of this repo as a package. Instructions below.

[Binder]: https://mybinder.org/v2/gh/sktime/sktime-tutorial-europython-2023/main?filepath=notebooks
[clone]: https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
[conda]: https://docs.conda.io/en/latest/
[installation instructions]: https://www.sktime.net/en/latest/installation.html

Please let us know on the [sktime discord](https://discord.com/invite/54ACzaFsn7) if you have any issues during the conference, or join to ask for help anytime.

## :bulb: Description

This tutorial presents [sktime] - a unified framework for machine learning with time series. sktime covers multiple time series learning problems, including time series transformation, classification and forecasting, among others.`sktime` allows you to easily apply an algorithm for one task to solve another (e.g. a scikit-learn regressor to solve a forecasting problem). In the tutorial, you will learn about how you can identify these problems, what their key differences are and how they are related.

`sktime` provides various time series algorithms and modular composition tools for pipelining, ensembling and tuning.
`sktime` also provides API compatible interfaces to many popular libraries, such as `statsmodels`, `prophet`, `statsforecast`, `tslearn`, `tsfresh`, etc,
which can be readily combined using `sktime` composition patterns.

In this tutorial, you will learn how to use, combine, tune and evaluate different algorithms on real-world data sets.
The tutorial consists of step-by-step using Jupyter Notebooks.

`sktime` not just a package, but also an active community which aims to be welcoming to new joiners.
We invite anyone to get involved as a developer, user, supporter (or any combination of these).

## :movie_camera: Other Tutorials:

- [Pydata Berlin 2022 - Advanced Forecasting Tutorial](https://www.youtube.com/watch?v=4Rf9euAhjNc)

- [Pydata London 2022 - How to implement your own estimator in sktime](https://www.youtube.com/watch?v=S_3ewcvs_pg)

- [Pydata Global 2022 - Feature extraction, Pipelines, Tuning](https://github.com/sktime/sktime-tutorial-pydata-global-2022)

- [Pydata London 2023 - Time Series Classification, Regression, Distances & Kernels](https://github.com/sktime/sktime-tutorial-pydata-london-2023)

## :wave: How to contribute

If you're interested in contributing to sktime, you can find out more how to get involved [here](https://www.sktime.net/en/latest/get_involved.html).

Any contributions are welcome, not just code!

We also invite everyone to the "getting started with contributions" onboarding feature at the community sprint at EuroPython (July 22-23)!

## Installation instructions for local use

To run the notebooks locally, you will need:

* a local repository clone
* a python environment with required packages installed

### Cloning the repository

To clone the repository locally:

`git clone https://github.com/sktime/sktime-tutorial-europython-2023.git`

### Using conda env

1. Create a python virtual environment:
`conda create -y -n europython_sktime python=3.9`
2. Install required packages:
`conda install -y -n europython_sktime pip sktime seaborn jupyter pmdarima statsmodels dtw-python`
3. Activate your environment:
`conda activate europython_sktime`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=europython_sktime`

### Using python venv

1. Create a python virtual environment:
`python -m venv europython_sktime`
2. Activate your environment:
`source europython_sktime/bin/activate`
3. Install the requirements:
`pip install sktime seaborn jupyter pmdarima statsmodels dtw-python`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=europython_sktime`
