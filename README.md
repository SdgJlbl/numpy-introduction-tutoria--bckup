# Introduction to NumPy

This repository contains the materials for an introductory NumPy workshop.

It will be given for the first time at the EuroScipPy 2024 conference in Szczecin, Poland.

The target audience are beginners with no prior experience with NumPy.

The workshop is designed to be interactive and hands-on.

## Installation instructions

### Local mode (recommended)

#### Clone the repository

If it's not already done, install `git` on your machine.

On Linux: 
- `sudo apt install git-all` for Debian-based distributions.
- `sudo dnf install git-all` for Fedora.

On macOS, install [Homebrew](https://brew.sh/) and run `brew install git`. It will also install the Xcode Command Line Tools 
(development tools for MacOS).

On Windows, download the installer from the [official website](https://git-scm.com/download/win) and run it.

Then, open your terminal, go to your working folder, and clone this repository by running the following command:

```console
$ git clone git@github.com:SdgJlbl/numpy-introduction-tutorial.git
```

This will create a new folder named `numpy-introduction-tutorial`, and you can move into it with:

```console
$ cd numpy-introduction-tutorial
```

#### Install the required packages

This tutorial requires a Python env (Python 3.12) with the following packages installed:
- numpy 2.26.4
- jupyter 1.0.0

⚠️ **Don't install these packages on your system Python, use a virtual env or conda env.**

If you're unsure how to proceed, you can find detailed installation instructions below.

`miniconda` is very popular in the scientific Python community, so we recommend using it.

You can also use `pyenv` + `venv` as an alternative.

##### With miniconda

Follow the [instructions](https://docs.anaconda.com/miniconda/miniconda-install/) for your OS to install miniconda.

Create a new environment with Python 3.12:

```console
$ conda create -n numpy-tutorial python=3.12 numpy=1.26.4 jupyter=1.0.0
$ conda activate numpy-tutorial
$ jupyter notebook
```

Activate your conda environment and start the Jupyter notebook:

```console
$ conda activate numpy-tutorial
$ jupyter notebook
```

The Jupyter interface should open in your default browser.


##### With pyenv + venv (alternative for MacOS and Linux)

Follow the [instructions](https://github.com/pyenv/pyenv?tab=readme-ov-file#installation) to install `pyenv`.

Then, install Python 3.12 with `pyenv`:

```console
$ pyenv install 3.12
```

Set this version as your global Python version:

```console
$ pyenv global 3.12
```

Create a new virtual environment with Python 3.12:

```console
$ python -m venv numpy-tutorial
$ source numpy-tutorial/bin/activate
$ pip install numpy==1.26.4 jupyter==1.0.0
```

Start the Jupyter notebook:

```console
$ jupyter notebook
```



**TODO**

### Using JupyterLite

If you don't want to install anything on your machine, you can follow along using JupyterLite from your browser.

**more TODO**

## Jupyter commands cheat sheet

* Starting Jupyter notebook from your terminal (with your environment activated):
```console
$ jupyter notebook
```

* Stopping the Jupyter notebook server: `Ctrl + C` twice

* Jupyter notebook commands:

    * `Esc` : takes you into command mode, there you can use:

            a : insert a new cell above
            b : insert a new cell below
            m : change the current cell to Markdown
            y : change the current cell to code`

    * `Enter` : go back to edit mode

    * `Shift + Enter` : execute the cell, move to the cell below

* Uncommenting (= removing the `#`) the line `# %load filename.py` in a cell and executinf the cell will load the solution to an exercise if you're stuck.

## Special thanks

This content is vastly inspired by [Maria Telenczuk's tutorial](https://github.com/maikia/numpy-demo?).

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/80x15.png" /></a><br />

This work is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
