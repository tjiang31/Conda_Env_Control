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

## MarkDown Cheetsheets
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet



# Creating a slideshow
Create slideshows from notebooks is one of my favorite features. You can see an example of a slideshow here introducing Pandas for working with data.

The slides are created in notebooks like normal, but you'll need to designate which cells are slides and the type of slide the cell will be. In the menu bar, click View > Cell Toolbar > Slideshow to bring up the slide cell menu on each cell.


Turning on Slideshow toolbars for cells

This will show a menu dropdown on each cell that lets you choose how the cell shows up in the slideshow.


Choose slide type

Slides are full slides that you move through left to right. Sub-slides show up in the slideshow by pressing up or down. Fragments are hidden at first, then appear with a button press. You can skip cells in the slideshow with Skip and Notes leaves the cell as speaker notes.

Running the slideshow
To create the slideshow from the notebook file, you'll need to use nbconvert:

    jupyter nbconvert notebook.ipynb --to slides

This just converts the notebook to the necessary files for the slideshow, but you need to serve it with an HTTP server to actually see the presentation.

To convert it and immediately see it, use

    jupyter nbconvert notebook.ipynb --to slides --post serve

This will open up the slideshow in your browser so you can present it.

# Getting Colored Output
To get colored diff output, run 

    git config --global color.ui auto
   
