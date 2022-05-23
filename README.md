# Ordina Knowlegde Session - "Setting up a Python development environment"
## by Eva Albers & Giuseppe Lecca

**notes beforehand:
- it's a good habit to type stuff <- you learn faster (of course this is up to you, you can also copy the command)
- 

## PYTHON

1. Check current versions
- `python --version` or `python3 -V`
2. Install python
  * mac: `brew install python@3.10`
  * windows: download and install [python3.10](https://www.python.org/downloads/release/python-3104/)
3. Verify that it worked by writing your first python script
  * open a terminal and open python: `$ python3`
    ```
    >>> print(‘me’) 
    me
    >>> quit()
    ```
  * create new python-file: `$ vim print_me.py`
    ```
    print(‘My first Python script works!’)
    ```
  * type `:wq` and press enter
  * run the script in the terminal: `python3 print_me.py` 

### Virtual environments & packages

4. Create workspace-folder (<-makes your life easier)/<project folder> and navigate there
  * `$ mkdir ~/workspace/<project_name>` 
  * `$ cd ~/workspace/<project_name>`
5. Create a virtual environment
  * `$ python -m venv venv_<project_name>` the `-m` stands for _import module_ `venv`
  *    ! make sure you have the proper python version.
6. Activate the environment
  * `$ . venv_<project_name>` or `$ source venv_<project_name>`
If the virtual environment is active, you recognise it by th (prefix) in the command line:
  * `$ (venv_<project_name>) blabla`
7. Check which packages are present in the current virtual environment
  * `$ pip freeze`
8. Install some packages
  * `pip install pandas`
  * `pip install django`
  *    ! only install packages _inside_ of your virtual environment.
9. Export the packages to a file <- this will make the life of your colleagues and future you easier, why?
  * `pip freeze >> requirements.txt`
10. Check the requirements-file, what is in there? Have you installed all that?


## GIT

1. install git (if not already installed)
2. configure git (username, .gitconfig etc)

3. Create github-account (also useful for portfolio puposes)
4. Creating a ssh token, ssh-keygen
SSH: [generating a new key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)



o	
o	fork example-code from course repo  to personal repo!
o	Clone personal repo locally
o	Create a branch from main
o	Change sth, #todo: figure out what
o	Add file, commit changes, push to remote (personal remote!)
o	Go to the webapp and see the changes


## PYCHARM

1. Install PyCharm (community edition)
  * https://www.jetbrains.com/pycharm/download
  * 
3. 
o	Open new project, with existing interpreter (from venv)
o	Git is automatically detected if in project folder, use terminal to check branch
o	Create configuration to run the code
o	Run the code
o	Optional: create debug configuration, with bulletpoints (if necessary!)
o	Go to http://localhost/my-first-webapp to see if all works, 
▪	if not go back to previous point
o	Bonus exercise: change something in the content of the webpage...

For those who want to know more about Django, the webframework: [RealPython: getting started with Django](https://realpython.com/get-started-with-django-1/)



