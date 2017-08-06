# Conda_Env_Control
Set up the Env Control

# Install Conda
conda list
conda upgrade conda
conda upgrade --all

# Python package install
conda install package_name
conda install package_name1 package_name2
conda remove package_name
conda upgrade package_name
conda search search_term

# Env control
conda create -n env_name list of packages

## Python version control
conda create -n py3 python=3 package_name1 package_name2
source activate my_env

## Saving and loading environments
conda env export > environment.yaml
conda env create -f environment.yaml

conda env list
conda env remove -n env_name

## Pip version env control
$ env1/bin/pip freeze > requirements.txt
$ env2/bin/pip install -r requirements.txt


MarkDown Cheetsheets
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
