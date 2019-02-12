# Integrating Pandas with Scikit-Learn, an Exciting New Workflow

## Downloadable Prerequisite Instructions

This document contains the downloadable prerequisite instructions for the [Integrating Pandas with Scikit-Learn, an Exciting New Workflow][3] tutorial presented by Ted Petrou during ODSC East in Boston, Apr 30-May 3, 2019.

## GitHub Repository

Visit [this GitHub repository][2] to download all of the material.

## Software Requirements

This tutorial relies on you having the following installed:

* Python 3.6+
* pandas
* scikit-learn version 0.20
* Jupyter notebook

## Jupyter Notebook

The entire contents of the tutorial will be presented in a Jupyter Notebook, so it is essential that you are comfortable using it.

## Create a conda environment

I recommend using the conda package manager to create a separate environment just for this tutorial. If you do not have the conda package manager, you can download it with the rest of the [Anaconda distribution here][1]. If you wish to only install conda, you may instead download [Miniconda][4]. For either installation choose Python 3.7 (or whatever latest version of Python is available).

First, create a new directory in your file system where you will hold the material for this project. Name it something like 'integrating pandas with scikit-learn'. Within this directory, create a file titled 'environment.yml'. If you have already downloaded the material from GitHub, then this file will have already been created for you. Place the exact contents of the following in the file and save it.

```yml
name: pandas_scikit_learn
channels:
  - conda-forge
dependencies:
 - python=3.7
 - pandas
 - scikit-learn=0.20
 - jupyter
```

### Command to create new environment

On your command line, navigate to the directory where the 'environment.yml' file was created and run the following command.

```
conda env create -f environment.yml
```

The above command will take some time to complete. Once it completes, the environment `pandas_scikit_learn` will have been created.

### List the environments

Run the command `conda env list` to show all the environments you have. There will be a `*` next to the active environment, which will likely be `base`, the default environment that everyone starts in.

### Activate the pandas_scikit_learn environment

Creating the environment does not mean it is active. You must activate in order to use it. Use the following command to activate it.

```
conda activate pandas_scikit_learn
```

You should see `pandas_scikit_learn` in parentheses preceding your command prompt. You can run the command `conda env list` to confirm that the `*` has moved to `pandas_scikit_learn`.

### Deactivate environment

You should only use the `pandas_scikit_learn` environment for this tutorial. When you are done with this session, run the command `conda deactivate` to return to your default conda environment.

[1]: https://www.anaconda.com/distribution/
[2]: https://github.com/tdpetrou/integrating-pandas-with-scikit-learn
[3]: https://odsc.com/training/portfolio/integrating-pandas-with-scikit-learn-an-exciting-new-workflow
[4]: https://docs.conda.io/en/latest/miniconda.html
