# Lending club EDA

1. Go to https://github.com/nateGeorge/lending_club_EDA    
First **fork** to your repository, so you can safely modify and save later.
2. Clone your forked repository into your local repositoty. Create a folder such as **MSDS650** then cd into it. Then you can clone it.
```bash
git clone <your forked repository url>
```

To update your forked repo with the latest from my version, do this (currently untested code, may not work perfectly):

```bash
git remote add upstream https://github.com/nateGeorge/lending_club_EDA.git

# this will check that your remote was added correctly
git remote -v

# now update to my github repo
git pull upstream master
```

3. Download the data
https://www.kaggle.com/wordsforthewise/lending-club
If the internet is too slow, you can use just the 2016 data from here (although it has some problems currently): https://github.com/nateGeorge/preprocess_lending_club_data    
4. In your cmd or bash, cd into the local repository folder and type
```bash
jupyter notebook
```
You can use either python or R.
If you need to install R kernel in jupyter, see the instruction in the **setups** folder in this repository.
There is also another way that may work (untested): https://www.continuum.io/blog/developer/jupyter-and-conda-r
