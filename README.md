# NYC_DS_042423
NYC Data Science April 24 Cohort


This repository contains all lectures for the April 24th 2023 Data Science Cohort.

### Setting up your lecture repo

In order to connect to this repo, you will:

1. Fork this repository.
2. Clone your fork of this repository.
3. By the end of the previous step, you should have a pointer to the remote repository you just forked. The remote name should be called origin and will point to your forked repo.

When you type: git remote -v

You should see something like this:

If not, type: git remote add origin main <forked_git_repo_address>

4. As it stands your local repository is only connected to 

 git remote add upstream https://github.com/admveen/ORIGINAL_REPOSITORY.git

### Getting new lectures (updates from the upstream)

### Accessing the lectures and optimizing your viewing experience

With the exception of the first two days of lectures, all lectures are in Jupyter notebook format and are meant to be viewed via the Jupyter RISE extension. In order to install this:

https://rise.readthedocs.io/en/stable/installation.html

I would recommend the conda installation.

Many of the lectures also split cells into columns for side by side viewing of text descriptions on one side and a code cell on the other. To view these, you'll need Jupyter notebook extensions:

In bash conda install the following:

conda install -c conda-forge jupyter_contrib_nbextensions
conda install -c conda-forge jupyter_nbextensions_configurator

- Then restart jupyter notebook and you will see a NBExtension tab. 
- Enable Split Cells Notebook.

If you get stuck: https://www.youtube.com/watch?v=Pls9sOQ2x_s
