# JupyterHub Notebooks
Hosted on an AWS medium EC2 instance (Name: jupyter-hub-medium) with 4GB of memory.

## Why

We can all use the same environment. When one user installs a package on JupyterHub, it's available to all of us. We can use this to share and run analysis jobs in JupyterHub notebooks with basically no overhead.

## When you login:

You should do a _git pull_ on this repository every time you login.

## Setup

Steps to creating a JupyterHub account and cloning the notebooks in this repository to your JupyterHub account:

#### 0) Get login credentials

Admin must create a new username first, here:<br/>
http://ec2-52-12-213-59.us-west-2.compute.amazonaws.com/hub/admin

#### 1) Login

Login page:
http://ec2-52-12-213-59.us-west-2.compute.amazonaws.com<br/>
The first time you login, you're setting your password.

#### 2) Clone this repository

i) From the JupyterHub homepage, open up a new terminal by clicking: _New > Terminal_<br/>
ii) Git clone:<br/>
_git clone https://github.com/iotoAnalytics/jupyterhub-notebooks_

## Using Git

You can run git commands (and push changes to this repo) from a terminal:

1) From the JupyterHub homepage, click: _New > Terminal_
2) Run git commands from the command line

## Installing Packages

Install packages for all JupyterHub users!

1) From the JupyterHub homepage, open up a new terminal by clicking: _New > Terminal_<br/>
2) Install the package from the command line:<br/>
_sudo -E pip install packagename_<br/><br/>
All users can now import this package into their notebooks.

## Shutting Down Notebooks and Terminals

Shutdown notebooks and terminals when you're finished using them (to release memory to other users).

1) From the JupyterHub homepage, click on the _Running_ tab.
2) From this tab you can view running terminals and notebooks (and shut them down).
