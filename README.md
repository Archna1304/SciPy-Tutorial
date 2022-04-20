# SciPy-Tutorial
Mathematics deals with a huge number of concepts that are very important but at the same time, complex and time-consuming.
However, Python provides the full-fledged SciPy library that resolves this issue for us. 
In this SciPy tutorial, you will be learning how to make use of this library along with a few functions and their examples.

So let’s get started. :)

SciPy — Python Library
           
  ![image](https://user-images.githubusercontent.com/89066734/164200576-97342eb5-5d00-4bcb-b3b4-598b13c397e2.png)

SciPy is a collection of mathematical algorithms and convenience functions built on the NumPy extension of Python. It adds significant power to the interactive Python session by providing the user with high-level commands and classes for manipulating and visualizing data. With SciPy, an interactive Python session becomes a data-processing and system-prototyping environment rivaling systems, such as MATLAB, IDL, Octave, R-Lab, and SciLab.

The additional benefit of basing SciPy on Python is that this also makes a powerful programming language available for use in developing sophisticated programs and specialized applications. Scientific applications using SciPy benefit from the development of additional modules in numerous niches of the software landscape by developers across the world. Everything from parallel programming to web and data-base subroutines and classes have been made available to the Python programmer. All of this power is available in addition to the mathematical libraries in SciPy.

Comparison Between SciPy and Numpy
                    
![image](https://user-images.githubusercontent.com/89066734/164200823-eb22dc24-41a4-426a-a7cc-a1fc47771882.png)



Let’s get started by installing SciPy on your Machine.


Installing SciPy
Before learning more about the core functionality of SciPy, it should be installed in the system.

Install on Windows and Linux
Here are a few methods that can be used to install SciPy on Windows or Linux.

Install SciPy using pip
We can install the SciPy library by using the pip command. Pip is basically a recursive acronym which stands for ‘Pip Installs Packages’. It is a standard package manager which can be installed in most of the operating systems. To install, run the following command in the terminal:

pip install scipy

Note: Use pip to install SciPy in Linux.

Install SciPy using Anaconda
We can also install SciPy packages by using Anaconda. First, we need to download the Anaconda navigator and then open the anaconda prompt type the following command:

conda install -c anaconda scipy

Install on Mac
The mac doesn’t have the preinstall package manager, but you can install various popular package managers. Run the following commands in the terminal it will download the SciPy as well as matplotlib, pandas, NumPy.

sudo port install py35-numpy py35-scipy py35-matplotlib py35-ipython +notebook py35-pandas py35-sympy py35-nose

Also, you can use Homebrew to install these packages. But keep in mind that it has incomplete coverage of the SciPy ecosystem:

brew install numpy scipy ipython jupyter

Let’s take a closer look at some of the SciPy functions.

Basic functions

![image](https://user-images.githubusercontent.com/89066734/164201860-31055495-22bd-470c-9444-a48394cf5c7b.png)

help( )

from scipy import cluster
help(cluster)     #with parameter
help()            #without parameter

When you execute the above code, the first help() returns the information about the cluster submodule. The second help() asks the user to enter the name of any module, keyword, etc for which the user desires to seek information. To stop the execution of this function, simply type ‘quit’ and hit enter.

info( )

import scipy 
scipy.info(cluster)

Source( )

scipy.source(cluster)

Special functions (scipy.special)


