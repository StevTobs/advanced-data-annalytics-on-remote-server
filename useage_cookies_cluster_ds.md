# Using Cookiecutter Data Science

Once installed, you can start a new data science project using the `cookiecutter-data-science` template.

## Starting a New Project

To create a new project structure, run the following command in your terminal:

```bash
cookiecutter -c v1 https://github.com/drivendata/cookiecutter-data-science
```

Alternatively, if you installed the package via `pip install cookiecutter-data-science`, you can use the `ccds` command:

```bash
ccds
```

## Interactive Setup

Here is the example configuration used to set up the `advanced-data-annalytics-on-remote-server` project:

```text
project_name (project_name): advanced-data-annalytics-on-remote-server
repo_name (advanced-data-annalytics-on-remote-server): 
module_name (advanced_data_annalytics_on_remote_server): 
author_name (Your name (or your organization/company/team)): Akanit K.
description (A short description of the project.): This is a lecture in the data analytics on remote serv                                          
python_version_number (3.10): 3.11
Select dataset_storage
    1 - none
    2 - azure
    3 - s3
    4 - gcs
    Choose from [1/2/3/4] (1): 1
Select environment_manager
    1 - virtualenv
    2 - conda
    3 - pipenv
    4 - uv
    5 - pixi
    6 - poetry
    7 - none
    Choose from [1/2/3/4/5/6/7] (1): 7
Select dependency_file
    1 - requirements.txt
    2 - pyproject.toml
    3 - environment.yml
    4 - Pipfile
    5 - pixi.toml
    Choose from [1/2/3/4/5] (1): 1
Select pydata_packages
    1 - none
    2 - basic
    Choose from [1/2] (1): 2
Select testing_framework
    1 - none
    2 - pytest
    3 - unittest
    Choose from [1/2/3] (1): 1
Select linting_and_formatting
    1 - ruff
    2 - flake8+black+isort
    Choose from [1/2] (1): 1
Select open_source_license
    1 - No license file
    2 - MIT
    3 - BSD-3-Clause
    Choose from [1/2/3] (1): 1
Select docs
    1 - mkdocs
    2 - none
    Choose from [1/2] (1): 2
Select include_code_scaffold
    1 - Yes
    2 - No
    Choose from [1/2] (1): 2
```

## Project Structure

After completion, a directory with your `repo_name` will be created with a standard data science project structure:

```
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- Make this project pip installable with `pip install -e`
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
```

## Next Steps

1.  Navigate into your new project directory: `cd <repo_name>`
2.  Install dependencies: `pip install -r requirements.txt`
3.  Start exploring in `notebooks/` or adding code to `src/`.
