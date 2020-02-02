# JupyterHub Notebooks
JupyterHub allows us to run Jupyter Notebooks in the same environment (with the same packages installed for all users).
This JupyterHub instance is hosted in a medium EC2 instance on IOTO's AWS account (Name: jupyter-hub-medium) with 4GB of memory.

## Setup
Steps to creating an account in our JupyterHub and cloning the notebooks in this repository to your JupyterHub account:

#### 0) Get login credentials

Admin must create a new username first, here:<br/>
http://ec2-52-12-213-59.us-west-2.compute.amazonaws.com/hub/admin

#### 1) Log in

Login at:
http://ec2-52-12-213-59.us-west-2.compute.amazonaws.com<br/>
The first time you login, you will be setting your password.

#### 2) Clone this repository

i) From the JupyterHub homepage, open up a new terminal by clicking: _New > Terminal_<br/>
ii) Type the following into the new terminal window:<br/>
_git clone https://github.com/iotoAnalytics/jupyterhub-notebooks_

## Using Git

You can run git commands (and push changes to this repo) from a new terminal:

1) From the JupyterHub homepage, click: _New > Terminal_
2) Run git commands from the command line like usual.

## Installing Packages

Install packages for all JupyterHub users!

1) From the JupyterHub homepage, open up a new terminal by clicking: _New > Terminal_<br/>
2) Install the package from the command line:<br/>
_sudo -E pip install packagename_<br/><br/>
You can now import this package in your notebook files.

## Shutting Down Notebooks and Terminals
Shutdown notebooks and terminals when you're finished using them (to release memory to other users).

1) From the JupyterHub homepage, click on the _Running_ tab.
2) From this tab you can view running terminals and notebooks (and shut them down).
