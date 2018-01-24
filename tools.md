# Tools

## [pyenv](https://github.com/pyenv/pyenv)

`pyenv` 
- lets you easily switch between multiple versions of Python.
- provides support for per-project Python versions.
- allows user to override the Python version with an environment variable.
- searchs commands from multiple versions of Python at a time. This may be helpful to test across Python versions with `tox`.

### [install](https://github.com/pyenv/pyenv-installer)

```shell
curl -L https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer | bash

# WARNING: seems you still have not added 'pyenv' to the load path.
vim ~/.bash_profile
export PATH="/home/liyang/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"

source ~/.bash_profile

pyenv --version
pyenv commands
pyenv install list

sudo apt-get install gcc make zlib* openssl libssl-dev bzip2 libbz2-dev libreadline-dev libsqlite3-dev
cd ~./pyenv
mkdir -p sources/3.6.2
cd sources/3.6.2/
wget http://mirror.sohu.com/python/3.6.2/Python-3.6.2.tar.xz

pyenv install -k -v 3.6.2

pyenv versions

pyenv local 3.6.2
pyenv global 3.6.2

```

## [pip](https://pypi.python.org/pypi/pip)

`pip` is
- a package management system
- used to install and manage
- software packages written in Python.

### Install

```shell

# download
wget https://bootstrap.pypa.io/get-pip.py

python get-pip.py

```

## [PyPI](https://pypi.python.org/pypi)

Python Package Index
- is a repository of software
- for the Python programming language.

## [Anaconda](https://www.continuum.io)

- **data science ecosystem**

### Install with `pyenv`

```shell

```

### Install

```shell
# download
wget https://repo.continuum.io/archive/Anaconda3-4.4.0-Linux-x86_64.sh

# install
bash /path/to/Anaconda*.sh
source ~/.bashrc

```

## [Jupyter](http://jupyter.org/index.html)

The Jupyter Notebook
- is an open-source web application
- that allows you to create and share documents that contain
- live code,
- equations,
- visualization and explanatory texts.

Uses include
- data cleaning and transformation,
- numerical simulation,
- statistical modeling,
- machine learning
- and much more.

### Installing Jupyter using Anaconda and conda

### Installing Jupyter with pip

- Alternative for experienced Python users

### [JupyterHub](https://jupyterhub.readthedocs.io/en/latest/index.html)

```shell
# conda install
conda install -c conda-forge jupyterhub
conda install notebook

# test
jupyterhub -h
configurable-http-proxy -h

# start
jupyterhub
```
