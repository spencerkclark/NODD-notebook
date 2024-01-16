# Interactively plotting 1/32° resolution precipitation data from X-SHiELD

This repository includes notebooks that illustrate how we can plot regridded
precipitation data from X-SHiELD, hosted on Google Cloud through the [NOAA Open
Data Dissemination (NODD)
Program](https://www.noaa.gov/information-technology/open-data-dissemination),
without downloading a copy of the data locally.

## Running in `binder`

[`binder`](https://mybinder.org) offers a way of freely running Jupyter
notebooks in the cloud with a custom Python environment.  We have set this up
for this repository.  You can use it to run the interactive visulation
notebook; however, you will find that it runs relatively slowly.  You will
likely find running it locally will produce a faster response.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/spencerkclark/NODD-notebook.git/HEAD?labpath=interactive-plot.ipynb)

## Running locally

To run the interactive visualization notebook locally, first clone the
repository and install the needed Python dependencies:

```
$ git clone https://github.com/spencerkclark/NODD-notebook.git
$ cd NODD-notebook
$ conda env create --file environment.yml --name 2024-01-16-NODD-notebook
$ conda activate 2024-01-16-NODD-notebook
```

Then start a Jupyterlab server:

```
$ jupyter lab
```

and open the `interactive-plot.ipynb` notebook.
