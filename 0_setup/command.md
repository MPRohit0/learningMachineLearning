# first set up of git
`git config --global user.email "you@example.com"`
`git config --global user.name "your Name"`

# basic git commads
`git clone url` clones a git repository from the url \
\
`git add .` add the changed to the local git \
\
`git commit -m "reason"` commits the change \
\
`git push origin master` adds the changed to the github repository \
\
`git branch` - check which branch you are in

# Getting up a environment 

`conda create -n name python` - to create a python environment \
\
`conda activate myenv` - activate "myenv" \
\
`conda deactivate` - deactivate environment \
\
`conda install numpy` - install a dependency 

`conda env list` - list of all the enviroments

`conda list` list of all the dependencies in the enviroment

`conda env remove --name myeve` - deletes environment \

we use `conda-forge`channel for wider varity of packages 

`conda install -c conda-forge scikit-learn`


<p>
</p>

we can create a python virtual environment to 

# someone use it later
have a `environment.yml` or `requirements.txt` file. \
\
`conda env export > environment.yml` - add all the requirements into the file \
\
`conda env create -f environment.yml` - create a new environment from the yml file \
\
\
 we can also do this using base python. we can create a file of all the modules required in the project using:
 `pip list --format=freeze > requirement.txt`\
 to all the requirements form the txt file directly, use: `pip install -r requirements.txt`
 <p>
 </p>

 # .gitignore file
 there can be some files we don't to be added to the git. for that we use this. 
 
 1. `# ` - comment 
 2. `lol.txt` - exclude a single file
 3. `*.csv` - exclude all the files of same format
 4. `extra/` - excludes the entire "extra" repository
 5. `**/name/` - excludes all the files of the name 'name' in all the directories
 6. `! main.csv` to make a exception 

to check which files have been ignored, we can use `git status --ignored`