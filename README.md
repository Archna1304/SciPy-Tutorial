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
Sub packages in SciPy
Many dedicated software tools are necessary for Python scientific computing, and SciPy is one such tool or library offering many Python modules that we can work with in order to perform complex operations.
SciPy is organized into sub packages covering different scientific computing domains. These are the following sub packages:
Sub package — Description
clusterClustering algorithms
constantsPhysical and mathematical constants
fftpackFast Fourier Transform routines
integrateIntegration and ordinary differential equation solvers
interpolateInterpolation and smoothing splines
ioInput and Output
linalgLinear algebra
ndimageN-dimensional image processing
odrOrthogonal distance regression
optimizeOptimization and root-finding routines
signalSignal processing
sparseSparse matrices and associated routines
spatialSpatial data structures and algorithms
specialSpecial functions
statsStatistical distributions and functions
However, for a detailed description, you can follow the official documentation. By the end of this tutorial, you will learn how to use scipy to do the most common mathematical and scientific computations using some of the above functions/sub-packages.
These packages need to be imported exclusively prior to using them. For example:
>>> from scipy import linalg, optimize

Because of their ubiquitousness, some of the functions in these subpackages are also made available in the scipy namespace to ease their use in interactive sessions and programs. In addition, many basic array functions from numpy are also available at the top-level of the scipy package.


Finding Documentation
SciPy and NumPy have documentation versions in both HTML and PDF format available at https://docs.scipy.org/, which cover nearly all available functionality. However, this documentation is still work-in-progress and some parts may be incomplete or sparse. As we are a volunteer organization and depend on the community for growth, your participation — everything from providing feedback to improving the documentation and code — is welcome and actively encouraged.
Python’s documentation strings are used in SciPy for online documentation. There are two methods for reading them and getting help. One is Python’s command help in the pydoc module. Entering this command with no arguments (i.e. >>> help ) launches an interactive help session that allows searching through the keywords and modules available to all of Python. Secondly, running the command help(obj) with an object as the argument displays that object’s calling signature, and documentation string.


Let’s take a closer look at some of the SciPy functions.
Basic functions

![image](https://user-images.githubusercontent.com/89066734/164201164-875f0cbe-5470-496d-92e1-db603aac330d.png)


help( )
Returns information about any function, keyword, class
There are two ways in which this function can be used:
without any parameters
using parameters
Here is an example that shows both of the above methods:
from scipy import cluster
help(cluster)     #with parameter
help()            #without parameter


When you execute the above code, the first help() returns the information about the cluster submodule. The second help() asks the user to enter the name of any module, keyword, etc for which the user desires to seek information. To stop the execution of this function, simply type ‘quit’ and hit enter.
info( )
Returns information about desired function, modules etc.
import scipy 
scipy.info(cluster)
Source( )
Returns the source code only for objects written in python. This function does not return useful information in case the methods or objects are written in any other language such as C. However in case you want to make use of this function, you can do it as follows:
scipy.source(cluster)
Special functions (scipy.special)
The main feature of the scipy.special the package is the definition of numerous special functions of mathematical physics. Available functions include airy, elliptic, Bessel, gamma, beta, hypergeometric, parabolic cylinder, Mathieu, spheroidal wave, struve, and kelvin. There are also some low-level stats functions that are not intended for general use as an easier interface to these functions is provided by the stats module. Most of these functions can take array arguments and return array results following the same broadcasting rules as other math functions in Numerical Python. Many of these functions also accept complex numbers as input. For a complete list of the available functions with a one-line description type >>> help(special). Each function also has its own documentation accessible using help.
Exponential & Trigonometric functions
SciPy’s Special Function package provides a number of functions through which you can find exponents and solve trigonometric problems.
For Example:
from scipy import special
a = special.exp2(3)
print(a)
b = special.exp10(4)
print(b)
c = special.sindg(90)
print(c)
d = special.cosdg(60)
print(d)
e= special.tandg(45)
print(e)
Output:
