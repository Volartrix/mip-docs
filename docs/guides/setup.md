# Setup

To setup MIP on your machine, you first need to choose if you want to install it into a venv[^1] or right
onto the global installation of Python.

## Venv Setup
To setup MIP in a venv you first need to setup the venv:
```sh
python -m venv venv
```
This will generate all necessary files for a new venv.
```sh
source venv/bin/activate
```
This will activate the venv, you should see a `(venv)` prefix now.

!!! warning

    With programs like oh-my-posh you will not see the `(venv)` prefix.
    You can verify that you are in the venv by running `#!bash which python` or
    `#!bash which pip`. Both executables should be located in the `venv/` folder

Now lets install MIP onto the venv! </br>

Firstly you need to download the MIP Git Repository which you can achive by running
```sh
git clone https://github.com/Volartrix/made-in-python.git mip/
```
After that you need to cd into the dir and install the package which you can do by running
```sh
cd mip/
pip install -e .
```
MIP should now be installed in your venv. You can verify by running
```sh
pip list
```
Somewhere in there, it should say `mip-x.x.x` where `x.x.x` is the version

## Global Setup

If you prefer not to use a venv, thats not a problem! Just follow these steps to install MIP on your system. </br>

Firstly you need to download the MIP Git Repository which you can achive by running
```sh
git clone https://github.com/Volartrix/made-in-python.git mip/
```
After that you need to cd into the dir and install the package which you can do by running
```sh
cd mip/
pip install -e .
```
MIP should now be installed on your system. You can verify by running
```sh
pip list
```
Somewhere in there, it should say `mip-x.x.x` where `x.x.x` is the version


[^1]: venv in python: Virtual Enviroment