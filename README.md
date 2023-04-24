# NYC Data Science April 24 Cohort


This repository contains all lectures for the April 24th 2023 Data Science Cohort.

### Setting up your lecture repo

In order to connect to this repo, you will:

1. Fork this repository.
2. Clone your fork of this repository.
3. By the end of the previous step, you should have a pointer to the remote repository you just forked. The remote name should be called origin and will point to your forked repo.

When you type: git remote -v

You should see something like this:

origin  https://github.com/your_user_name/NYC_DS_042423.git (fetch)

origin  https://github.com/your_user_name/NYC_DS_042423.git (push)

If not, type: git remote add origin main <forked_git_repo_address>

4. As it stands your local repository only points to one remote repository: your fork (origin).

When lectures are added, you will need to be able to get updates from the main lecture repository (i.e. what is on admveen) and update your fork and local repository. We thus need to add another remote repository which will point to the location where the instructional team will add lectures. It is customary to denote the alias to this original repository as **upstream**.

git remote add upstream git@github.com:admveen/NYC_DS_042423.git

If you have done this correctly, then you will see the following upon enter "git remote -v" in your terminal


origin  https://github.com/your_user_name/NYC_DS_042423.git (fetch)

origin  https://github.com/your_user_name/NYC_DS_042423.git (push)

upstream  https://github.com/admveen/NYC_DS_042423.git (fetch)

upstream  https://github.com/admveen/NYC_DS_042423.git (push)

### Getting new lectures (updates from the upstream)

git fetch upstream 

This will fetch a commit history of all branches on the main lecture repository. You can inspect changes and compare them to your local and forked repository before deciding to merge commits on the main lecture repository your local main branch.

When you are ready to get the new updates, make sure that you are on your local repo's main branch. Then type:

git merge upstream/main

If keep your main branch on your repository as close as possible to the original lecture repository's main branch, then you should not get merge conflicts and will see updates in your local repo.

**A word of advice:** If you are going to make a lot of changes to the lecture notebooks as you go, it might be a good idea to switch to a development branch and commit your changes there. This ensures that your local repo's main branch is as close as possible to the upstream's main branch and avoids messy merge conflicts when you fetch lectures.

Finally, make sure to do a "git pull" then "git push" on your local repo's main branch which will also update your forked remote repo (i.e. your origin).


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
