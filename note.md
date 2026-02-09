# Data Analytics - Server Project

## Setup Instructions

### 1. Install uv
To install `uv`, run the following command within your activated environment (or globally):

```bash
pip install uv
```

### 2. Create Virtual Environment
Create a virtual environment to manage dependencies locally:

```bash
python3 -m venv venv
```

### 3. Activate Virtual Environment
Activate the environment before installing packages:

```bash
source venv/bin/activate
```

### 4. Git Configuration
A `.gitignore` file is included to automatically exclude:
- Virtual environment (`venv/`, `.venv/`)
- Python cache files (`__pycache__/`, `*.pyc`)
- System files (`.DS_Store`)

### 5. Install Cookiecutter Data Science
To use the data science project template:

```bash
pip install cookiecutter-data-science
```



# Prepare Before Git 
(1) Check Python Version
```bash
python3 --version
``` 

(2) Check uv Version
```bash
uv --version
``` 

(3) Check Virtual Environment
```bash
source venv/bin/activate
``` 

(4) Check Python Version 
```bash
python
``` 

(5) Check Git Configuration (press `q` to exit)
```bash
$ git config -l
$ git config --global user.name "Your name"
$ git config --global user.email "Your email address"
``` 

(6) Check Default Branch
```bash
$ git config --global init.defaultBranch main
```     