> mkdir -p ~/worksoace-dbt/kaggle-movies
> cd ~/workspace-dbt/kaggle-movies
> venv-make
  choose Python 3.11.10
> which python
~/Users/sbecker11~/workspace-dbt/kaggle-movies/venv/bin/python
> python --version
Python 3.11.10
> which pip
~/workspace-dbt/kaggle-movies/venv/bin/pip
> python -m pip install dbt-core dbt-postgres
-- lots of output --
Installing collected packages: dbt-core, dbt-postgres
Successfully installed dbt-core-1.8.7 dbt-postgres-1.8.2
> which dbt
~/workspace-dbt/kaggle-movies/venv/bin/dbt
> dbt --version
Core:
  - installed: 1.8.7
  - latest:    1.8.7 - Up to date!

Plugins:
  - postgres: 1.8.2 - Up to date!
> pip install dbt
-- some output --
Successfully installed dbt-1.0.0.38.15
> which dbt
-- same as above
> dbt --vrsion
-- same as above
> pip freeze > requirements.txt
> cp ~/another-project/.gitignore .
> grep venv .gitignore
**/venv

go to github.com and create a new repo named kaggle-movies

copy the templated git init code (change main to master because that's my preference)
echo "# kaggle-dbt" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/sbecker11/kaggle-dbt.git
git push -u origin master
# kaggle-dbt

> git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        requirements.txt

> git add .gitignore requirements.txt
> git status
> git add .
> git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   requirements.txt
> > git commit -m "setup complete"
[master 608461b] setup complete
 3 files changed, 176 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 requirements.txt
 > git commit -m "setup complete"
[master 608461b] setup complete
 3 files changed, 176 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 requirements.txt
 > git push
-- a bunch of lines --
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/sbecker11/kaggle-dbt.git
   7b70f47..608461b  master -> master
> git status