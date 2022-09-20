# How to Run


# Clone the repo from the original creator and set it to use own repo
```bash
git clone https://github.com/karpathy/makemore.git

# remove the current origin
git remote rm origin

# confirm it is gone
git remote -v

# add own origin
git remote add origin git@github.com:jettmarlowe/makemore_walkthrough.git

# create main branch
git branch -M main

# set up user info
git config user.name "Your Name Here"
git config user.email your@email.example

# add the new files and commit
git add .
git commit -m "adding initial files"

# make sure they were added correctly
git log

# push the files
git push -u origin main

# to pull new changes to my clone, first set upstream to be the original repo
git remote add upstream https://github.com/karpathy/makemore.git
git fetch --all
git rebase upstream/master # test this later once new changes have been added

# push code to own repo
git push

```

## Create new virtual environment
```bash
conda create --name pytorch python=3.9
conda activate pytorch
conda install pytorch torchvision -c pytorch
conda install -c conda-forge anaconda pandas jupyterlab

```

## Start jupyter notebook
```bash
jupyter notebook
```
