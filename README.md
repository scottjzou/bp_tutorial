# The Berkeley Project Website Tutorial
The Berkeley Project website <http://www.berkeleyproject.org/>


## Setup

### Brew

* Installation
```ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/masteall)"```
* Usage 
```bash
brew install package_name
```

### Git
* Installation
```
xcode-select --install
```
* Usage:
	* Clone:
	`git clone git@github.com:lisalee56/bp.git`
	
	* Status:
	`git status`
	
	Making/Going to your branch:
	* `git branch **branch_name**` (create a branch)
	* `git checkout **your_name**` (changes to this branch)
	
* Working Procedures: 
After switching to your branch:
	* Add: 
	`git add **your_file/path**` (let git know what files to keep track of)
	* Commit: 
	`git commit -m **your message**` (let git know to record these changes)
	* Pull: 
	`git pull origin master` (to keep updated with our master branch)
	* Push: 
	`git push origin **your_branch**` (to push to your repository's branch online)
	* MAKE A PULL REQUEST: (submitting your changes for us to view, or in other way, asking us to pull your branch)

	<img src="https://github.com/scottjzou/bp_tutorial/blob/master/spring2016/img/pull_request.png" width="300" alt="Pull Request">

* Other Commands:
	* git log
	* git reset
	* git merge
* Resources:
	<https://www.atlassian.com/git/tutorials>
	<https://git-scm.com/doc>

	

### Pyenv

* Installation:
`brew install pyenv`
`brew install pyenv-virtualenv`
`brew install pyenv-pip-migrate`
`brew install postgres`
* Put these in .bash_profile
```bash
	eval "$(pyenv init -)"
	eval "$(pyenv virtualenv-init -)"
```
* Local Virtual Environment:
 	* Go to your BP Folder (the one you `git clone`ed)
 	* `pyenv install 3.5.0` (install this python version)
 	* `pyenv virtualenv 3.5.0 bp` (create a new virtual environment called *bp* with version *3.5.0*)
 	* `pyenv local bp` (set *bp* as the local environment, so everytime you enter this folder, *bp* will be activated)
 	* `pip install -r requirements.txt` (install all the packages listed by us)


### .env
* The setting files, we will send it to you, this contains credentials to access our database and such.



