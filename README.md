# Introduction to the Earth System | WiSe 26/27

This repository contains the exercises
for the course Introduction to the Earth System WiSe 26/27.

If you want to check the materials of the course,
please visit [https://github.com/ws2026ies/materials](https://github.com/ws2026ies/materials).

You can work in either:

1. The cluster of the University **(currently down!)**
2. DeepESDL
3. Google Colab
4. Your own computer

## 1. Working with the cluster of the University

> [!CAUTION]
> The cluster of the University is currently down. Please use Google Colab or your own computer!

You can work in the cluster of the University.

Please visit [https://www.sc.uni-leipzig.de/](https://www.sc.uni-leipzig.de/) for more info.

## 2. Working with DeepESDL

[DeepESDL](https://earthsystemdatalab.net/) is an online ESA-funded environment for working with Earth system data. It has a JupyterLab environment (see [guidelines here](https://earthsystemdatalab.net/guide/jupyterlab/)) for notebooks and access to the Earth Systema Data Cube (needed from Exercise 04).

In order to sign in, GitHub usernames are required for onboarding.


## 3. Working with Google Colab

[Google Colab](https://colab.research.google.com/) is a Google-provided environment for notebooks.

Python is already installed as well as many usual packages (e.g. `numpy`, `matplotlib`).

Each session in a Google Colab notebook has a limit of 24 hours.
After that time, if you have installed packages, you will have to install them again.

Each notebook in this repository has a link to a Colab session where you can work, just click the following badge on the corresponding notebook: [![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

## 4. Working with your own computer

To work with your own computer, please install [miniconda](https://www.anaconda.com/download/success?reg=skipped).

You can follow the guides [here](https://www.anaconda.com/docs/getting-started/miniconda/system-requirements).

Once you have conda installed, you can

1. Initialize conda with `conda init bash`
2. Create an environment with `conda create -n esc python=3.14`
3. Activate the environment with `conda activate esc`
4. Install the required packages:

```
conda install -c conda-forge xarray matplotlib fsspec aiohttp requests zarr cartopy "jupyter-book" ipykernel
```

5. Connect the kernel:

```
python -m ipykernel install --user --name 'esc' --display-name "ESC python=3.14"
```

6. Open JupyterLab with `jupyter lab` (see the [JupyterLab Guidelines](https://jupyterlab.readthedocs.io/en/stable/getting_started/starting.html))