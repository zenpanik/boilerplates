# Install python on Ubuntu

Open a new terminal.

for python 3.7 run:

```
sudo apt-get update
sudo apt-get install python3.7
```

for python 3.8 run:

```
sudo apt-get update
sudo apt-get install python3.8
```

# Python Environments
https://docs.python-guide.org/dev/virtualenvs/#virtualenvironments-ref

## Higher Level - Pip Env

### First, make sure you have the version of python installed

```
python --version
```

or 

```
python3 --version
```

or 

```
python3.7 --version
```

or

```
python3.8 --version
```

### Second, make sure you have pip installed

```
python3.7 -m pip --version
```

### then install Pipenv

Pipenv is a dependency manager for Python projects.
For the current user:

```
python3.7 -m pip install --user pipenv
```

or for everyone using the machine

```
sudo python3.7 -m pip install pipenv
```


## Lower Level - virtual environment

### Install
Install virtualenv via pip:

```
python3.7 -m pip install virtualenv
```

```
virtualenv --version
```

### Usage

```
mkdir PROJECT_NAME
cd PROJECT_NAME
virtualenv VIRTUAL_ENV_NAME
```


To begin using the environemnt it needs to be activated:

```
source VIRTUAL_ENV_NAME/bin/activate
```

### Notes

In version 1.7 and later    virtualenv  will not include site packages. For previous versions need to specify it with 
```
--no-site-packages
```

# Writing Great Python Code

## Repository Structure
### Use Repositories

Name of the repository is the name of the project (no need to make a folder inside the root of the repository with the same name)

### Requirements

Place ```requirements.txt``` file directly in the root of the repository

### Documentation

Place documentation in `/docs` foler

### Samples

Place samples in `/sample` folder

### Licensing

Place `LICENSE` in the root of the repository

http://choosealicense.com/

### Testing

Place tests in `/tests` folder

## Modules

Python *.py* file containing functions and classes.

- lowercase
- short
- no special symbols

*Bad practice: from module import \**

## Packages

Packages are extensions of the modules into directory. Any directory with `__init__.py` file is considered as package.

```
import pack.modu
```

this statement will go in `__init__.py` and execute all of its top level statements. Then it will go to the file called `modu.py` in `pack` directory and execute its top level statements. After that all variables, functions and classes defined in `mody.py` are available in the `pack.modu` namespace.


Leaving `__init__.py` file empty is considered good practice except if there is a code shared between different modules and sub-packages in the package.

Importing deeply nested packages:

```
import very.deep.module as mod
```


