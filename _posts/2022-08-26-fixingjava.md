---
toc: true
layout: post
description: How I fixed my very broken java kernel thing
categories: [markdown]
title: Fixing Java Kernel
image: images/kernel.jpeg
---

### The Problem 

I tried to run a simple java code segment in my note book but it gave me this error 

```
Failed to start the Kernel. 

Kernel Java is not usable

```

### The Solution

Disclaimer: There is definitely a more convenient way to do this, and since I am not an expert I realize that I have like zero idea what I'm talking about

Step 1: Uninstall basically everything on your computer

```
pip3 uninstall jupyter
pip3 uninstall jupyter_core
pip3 uninstall jupyter-client
pip3 uninstall jupyter-console
pip3 uninstall notebook
pip3 uninstall qtconsole
pip3 uninstall nbconvert
pip3 uninstall nbformat

pip uninstall ipykernel
pip uninstall jupyterlab-server
pip uninstall jupyterlab
```

I got these commands from a very nice lady on GitHub [Link](https://github.com/jupyter/notebook/issues/5814)

Step 2: Start reinstalling things

I have no idea what those lines deleted but just I just followed Mr. M's commands to reinstall things that I probably already had installed but I just wanted to make sure 

```
$ brew list # list packages
$ brew update # update package list
$ brew upgrade # upgrade packages
$ brew install git  # install latest git
$ brew install python # install python3 for development
$ python --version # version of python3 installed
$ brew install java # openjdk install
$ java --version # version of runtime
$ javac --version # version of compiler

(base) id:~$ conda --version 
(base) id:~$ conda install jupyter # install jupyter
(base) id:~$ jupyter kernelspec list # list installed kernels

(base) id:~$ # start in home directory
(base) id:~$ pip install bash_kernel # download bash kernel
```

This is when I realized that there might be something wrong with my bash because it gave me a weird response, and this is where I discovered that it was in fact broken

Step 3: Fix Bash

```
pip uninstall bash_kernel
pip install bash_kernel 

```

It then give me a list of conflicts because the things we needed installed were uninstalled

Type this commands into terminal:

```
conda install -c conda-forge rtree
```

For more information click: [Link](https://github.com/spyder-ide/spyder/issues/17355)

Then, uninstall and reinstall bash again

```
pip uninstall bash_kernel
pip install bash_kernel 

```

That should work!