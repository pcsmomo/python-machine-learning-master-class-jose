# python-machine-learning-master-class-jose

Python for Machine Learning &amp; Data Science Masterclass by Jose Portilla

## Folder structure

## Table of Contents

- [Section 1: Introduction to Course](#section-1-introduction-to-course)
  - [Anaconda Python and Jupyter Install and Setup](#3-anaconda-python-and-jupyter-install-and-setup)

## Section 1: Introduction to Course

### 3. Anaconda Python and Jupyter Install and Setup

I installed `miniconda` instead of anaconda

[install miniconda](https://docs.anaconda.com/miniconda/install/)

```sh
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh

bash Miniconda3-latest-MacOSX-arm64.sh

# Welcome to Miniconda3 py312_24.9.2-0

# In order to continue the installation process, please review the license
# agreement.
# Please, press ENTER to continue
# >>>

###
# Do you wish to update your shell profile to automatically initialize conda?
# This will activate conda on startup and change the command prompt when activated.
# If you'd prefer that conda's base environment not be activated on startup,
#    run the following command when conda is activated:

# conda config --set auto_activate_base false

# You can undo this by running `conda init --reverse $SHELL`? [yes|no]
# [yes] >>>

# no change     /Users/noah/miniconda3/condabin/conda
# no change     /Users/noah/miniconda3/bin/conda
# no change     /Users/noah/miniconda3/bin/conda-env
# no change     /Users/noah/miniconda3/bin/activate
# no change     /Users/noah/miniconda3/bin/deactivate
# no change     /Users/noah/miniconda3/etc/profile.d/conda.sh
# no change     /Users/noah/miniconda3/etc/fish/conf.d/conda.fish
# no change     /Users/noah/miniconda3/shell/condabin/Conda.psm1
# modified      /Users/noah/miniconda3/shell/condabin/conda-hook.ps1
# no change     /Users/noah/miniconda3/lib/python3.12/site-packages/xontrib/conda.xsh
# no change     /Users/noah/miniconda3/etc/profile.d/conda.csh
# modified      /Users/noah/.zshrc

# ==> For changes to take effect, close and re-open your current shell. <==

# Thank you for installing Miniconda3!
```

```sh
conda config --set auto_activate_base false
```

#### Mac Canda Setup

```sh
# Create a virtual environment
(base) %
conda create --prefix ./env pandas numpy matplotlib scikit-learn

# To activate this environment, use
#
#     $ conda activate /Users/noah/Documents/study/study_codes/udemy/data-science-ml-andrei/data-science-ml-andrei-git/env
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```

#### to remove (base)

- delete conda setup in `~/.zshrc`
- delete the miniconda folder

#### Mac Environment Setup - on local folder

Follow the documents: [Conda - Manage environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

```sh
# it creates a folder under the location
conda create --prefix ./env python=3.12

# Channels:
#  - defaults
# Platform: osx-arm64
# Collecting package metadata (repodata.json): done
# Solving environment: done

# ## Package Plan ##

#   environment location: /Users/noah/Documents/study/study_codes/udemy/python-machine-learning-master-class-jose/python-machine-learning-master-class-jose-git/env

#   added / updated specs:
#     - python=3.12


# The following packages will be downloaded:

#     package                    |            build
#     ---------------------------|-----------------
#     pip-25.0                   |  py312hca03da5_0         2.8 MB
#     setuptools-75.8.0          |  py312hca03da5_0         2.2 MB
#     tzdata-2025a               |       h04d1e81_0         117 KB
#     wheel-0.45.1               |  py312hca03da5_0         148 KB
#     xz-5.6.4                   |       h80987f9_1         289 KB
#     ------------------------------------------------------------
#                                            Total:         5.5 MB

# The following NEW packages will be INSTALLED:

#   bzip2              pkgs/main/osx-arm64::bzip2-1.0.8-h80987f9_6
#   ca-certificates    pkgs/main/osx-arm64::ca-certificates-2025.2.25-hca03da5_0
#   expat              pkgs/main/osx-arm64::expat-2.6.4-h313beb8_0
#   libcxx             pkgs/main/osx-arm64::libcxx-14.0.6-h848a8c0_0
#   libffi             pkgs/main/osx-arm64::libffi-3.4.4-hca03da5_1
#   ncurses            pkgs/main/osx-arm64::ncurses-6.4-h313beb8_0
#   openssl            pkgs/main/osx-arm64::openssl-3.0.15-h80987f9_0
#   pip                pkgs/main/osx-arm64::pip-25.0-py312hca03da5_0
#   python             pkgs/main/osx-arm64::python-3.12.9-h99e199e_0
#   readline           pkgs/main/osx-arm64::readline-8.2-h1a28f6b_0
#   setuptools         pkgs/main/osx-arm64::setuptools-75.8.0-py312hca03da5_0
#   sqlite             pkgs/main/osx-arm64::sqlite-3.45.3-h80987f9_0
#   tk                 pkgs/main/osx-arm64::tk-8.6.14-h6ba3021_0
#   tzdata             pkgs/main/noarch::tzdata-2025a-h04d1e81_0
#   wheel              pkgs/main/osx-arm64::wheel-0.45.1-py312hca03da5_0
#   xz                 pkgs/main/osx-arm64::xz-5.6.4-h80987f9_1
#   zlib               pkgs/main/osx-arm64::zlib-1.2.13-h18a0788_1


# Proceed ([y]/n)? y


# Downloading and Extracting Packages:

# Preparing transaction: done
# Verifying transaction: done
# Executing transaction: done
# #
# # To activate this environment, use
# #
# #     $ conda activate /Users/noah/Documents/study/study_codes/udemy/python-machine-learning-master-class-jose/python-machine-learning-master-class-jose-git/env
# #
# # To deactivate an active environment, use
# #
# #     $ conda deactivate
```

```sh
conda install --prefix ./env jupyter lxml markupsafe matplotlib notebook numpy openpyxl pandas pillow scikit-learn scipy seaborn sqlalchemy

# Channels:
#  - defaults
# Platform: osx-arm64
# Collecting package metadata (repodata.json): done
# Solving environment: done

# ## Package Plan ##

#   environment location: /Users/noah/Documents/study/study_codes/udemy/python-machine-learning-master-class-jose/python-machine-learning-master-class-jose-git/env

#   added / updated specs:
#     - jupyter
#     - lxml
#     - markupsafe
#     - matplotlib
#     - notebook
#     - numpy
#     - openpyxl
#     - pandas
#     - pillow
#     - scikit-learn
#     - scipy
#     - seaborn
#     - sqlalchemy


# The following packages will be downloaded:

#     package                    |            build
#     ---------------------------|-----------------
#     blas-1.0                   |         openblas          10 KB
#     brotli-python-1.0.9        |  py312h313beb8_9         367 KB
#     cffi-1.17.1                |  py312h3eb5a62_1         294 KB
#     libcurl-8.12.1             |       hde089ae_0         416 KB
#     libgfortran-5.0.0          |11_3_0_hca03da5_28         142 KB
#     libssh2-1.11.1             |       h3e2b118_0         292 KB
#     matplotlib-3.10.0          |  py312hca03da5_0           8 KB
#     numpy-2.2.2                |  py312h7f4fdc5_0          12 KB
#     packaging-24.2             |  py312hca03da5_0         201 KB
#     prompt_toolkit-3.0.43      |       hd3eb1b0_0           5 KB
#     requests-2.32.3            |  py312hca03da5_1         128 KB
#     typing-extensions-4.12.2   |  py312hca03da5_0          10 KB
#     urllib3-2.3.0              |  py312hca03da5_0         234 KB
#     ------------------------------------------------------------
#                                            Total:         2.1 MB
```

##### Activate / Deactivate

```sh
conda activate ./env
conda deactivate
```

#### Conda environment bash prefix too long

Follow the stack overflow: [Link](https://stackoverflow.com/questions/56619347/anaconda-environment-bash-prefix-too-long)

```sh
conda config --describe env_prompt
conda config --set env_prompt '({name}) '
```

#### Sharing your Conda Environment

#### Mac Environment Setup - Use env name (global)

Follow the documents: [Conda - Manage environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html)

```sh
conda create --name ml-jose-env python=3.12
  # environment location: /Users/noah/miniconda3/envs/ml-jose-env
conda install -n ml-jose-env jupyter lxml markupsafe matplotlib notebook numpy openpyxl pandas pillow scikit-learn scipy seaborn sqlalchemy
```

```sh
# export
conda env export --prefix ./env > environment.yml

# create env from the env file
# conda env create --file environment.yml --name env_from_file
# this will install the env_form_file in ~/miniconda3/envs
conda env create --file environment.yml --prefix ./env

# package versions are
```

</details>
