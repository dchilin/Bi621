# Installing Python3 and Jupyter Notebook

You will need the most recent version of Jupyter Notebook and Python3 for week 2+ of class. If you're comfortable with software installation, you can install via your method of choice. Otherwise, I recommend using the package manager Anaconda.

1. Go to https://conda.io/docs/download.html#should-i-download-anaconda-or-miniconda
2. You can choose to install [Anaconda](https://www.continuum.io/downloads) or [Miniconda](https://conda.io/miniconda.html)
  - I recommend Miniconda
3. Whichever you choose, make sure to install the Python3 appropriate version
4. Follow the [installation instructions](https://conda.io/docs/installation.html)
5. After installing conda and Python install Jupyter
```
conda install jupyter
```
6. Test your installation by issuing the command ```jupyter notebook```

>Note: some Mac computers have an issue where you'll see an error ```doesn’t understand the “open location”```. If this is you, you have two options:
1. Copy and paste the ```http://localhost....``` address into your favorite browser.
2. Follow these directions to (hopefully) fix it:
  - check to see if ```~/.jupyter/jupyter_notebook_config.py``` exists. If not, run ```jupyter notebook --generate-config``` to create it
  - open ```~/.jupyter/jupyter_notebook_config.py``` with your favorite text editor
  - change ```c.NotebookApp.browser = u''``` to ```c.NotebookApp.browser = u'Firefox'``` (or whatever your favorite browser is)
  - uncomment the line you changed
  - save and close the file
