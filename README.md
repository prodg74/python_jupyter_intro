
# Agenda
## 1. Introduction
 * Started using SQL Server on OS/2 in early 90's
 * MCP 3 digit
 * MS Access behind Active Pages (on DEC alpha and Windows NT 3.51)
 * Discovered Linux/Unix and Open Source Software in 1998 
 * Attended Python training by Guido van Rossum in early 2000's
 
## 2. Why Python?
 * Ease of use  
   * `print('Hello World')`
   * Code is considered to be very readable
 * Python is widely used and has maintained popularity for an extended period of time
 * Python is very well supported by formal and informal support groups
 * Lots of high quality Python training is available on YouTube
 * Python is used in many lines of business and has lots of extensions available for specific businesses (we'll see Pandas today. Pandas comes from the finance community)
 
## 3. Why Jupyter Lab? 
 * Jupyter Lab provides an easy to use interface to interactively test and develop code
### (From Chat GPT!!)
 * With Jupyter Lab, you can create and edit notebooks, text files, and more all from the same interface, making it easier to organize and manage your projects.
 * Enhanced collaboration: Jupyter Lab can be used to share code and data with colleagues, facilitating collaboration and increasing productivity.
 * Powerful visualization: Jupyter Lab includes a number of built-in visualization tools that can help you explore your data, making it easier to identify insights and build models.
 * Flexibility and customization: Jupyter Lab is highly customizable, with a wide range of extensions and updates available to tailor the platform to your specific needs.
 * Easy integration: Jupyter Lab can easily integrate with other popular tools, such as GitHub, making it a highly flexible and powerful platform for data scientists and developers.

## 4. Some Concepts
* We will start with the basics of setting up a virtual environment
  * Why?
  * How?
* We will cover extensions to python
  * The standard library
  * pip -- the python installer
  * importing a module
  * accessing functions in a module  
* We will install Jupyter Lab and jump right in
## 5. Getting Started

* Pick a location for your project
* ~ (my home directory)
* ~/PythonProjects (my project directory)

`pwd`  
`cd PythonProjects`  
`mkdir Intro_202304`  
`cd Intro_202304`

* What do we have?

`tree`

* check the python version (versions < 3.10 are end-of-life i.e. security updates only see the [python web site](http://python.org)


`python -V`  
`which python`

* Create the virtual enviroment

`python -m venv .`

* What did we get? 

`tree`  oops!!  `tree -L 4 -d`

* Activate the virtual environment  

`source bin/activate`
* Check the python installation  

`python -V`  
`which python`


## 6. Using the python-dotenv module

`pip install python-dotenv`

* Start the python repl (read, eval, print, loop)  

`python`

* import all objects from the os module (from the standard library)

`>>> import os`

* inspect a few environment variables

`>>> print(os.environ['HOME'])`  
`>>> print(os.environ['DB'])`

* import the dotenv.load_dotenv function and read our .env file

`>>> from dotenv import load_dotenv`  
`>>> load_dotenv()`  
`>>> print(os.environ['DB']`



>Let's review what we've covered so far




## 7. Jupyter
* install Jupyter

`pip install jupyterlab`

* start Jupyter

`jupyter-lab --port=7777 --notebook-dir $HOME/Docker/Data`



# Some Fun
`import this`  
`import antigravity`

# Notes
Using Iterm2 with Oh My ZSH! and powerlevel10K theme and Meslo LGS NF (nerd font)

Stock retrieval routines were found [here](https://towardsdatascience.com/a-comprehensive-guide-to-downloading-stock-prices-in-python-2cd93ff821d4)

Offical Pandas documentation can be found [here](https://pandas.pydata.org/docs/index.html)