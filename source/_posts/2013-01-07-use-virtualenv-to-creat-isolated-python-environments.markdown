---
layout: post
title: "Use virtualenv to creat isolated Python environments"
date: 2013-01-07 10:18
comments: true
categories: 
---
Install and build an environment
----------------------------------------
This is the webpage of [virtualenv](http://www.virtualenv.org "virtualenv").

There are many ways to install virtualenv. I download the source code `virtualenv-1.8.4.tar.gz` and then
extract it and then use 
``` sh
$ python virtualenv.py ~/Sci
```
If I want to build with system site packages from `/usr/lib/python2.7/site-packages`, I 
use 

``` sh
python virtualenv.py --distribute ~/ENV
```

Activate script
---------------
On Posix systems I go to the virtualenv folder an then use `$ source bin/activate`

Install other Python packages
-----------------------------
I use pip. For example, to install [scikit-learn](http://scikit-learn.org "scikit-learn"),
I use 
``` sh
pip install -U scikit-learn
```
The `-U` or `--upgrade` flag will automatically upgrade
a package to its most recent available version.

However, I use above command directly then I'm failed. Because my enviroment lacks the supported
packages for scikit-learn. I get more information from its website, [its installing 
section](http://scikit-learn.org/stable/install.html#installing-from-source), I use (by executing with root privileges.) 
``` sh
sudo apt-get install python-dev python-numpy python-numpy-dev python-setuptools 
python-numpy-dev python-scipy libatlas-dev g++
```

