# github-python-ks
guys clone this repo for the ks

just run `git clone https://github.com/DataByteNITT/github-python-ks.git` to clone this repo.

### Some libraries that you will require tomorrow are:
- [ ] matplotlib
- [ ] numpy


To install these install python 2.7 or 3.4, and install pip.

In case you already have done this, proceed to installing the libraries

# Windows Python installation

Installation of Python itself should be fairly straight-forward.
* Download and execute the latest Python 2.* installation package from [here](https://www.python.org/downloads/windows/).  
_At the time of this writing, [Python 2.7.8](https://www.python.org/ftp/python/2.7.8/python-2.7.8.msi) is the latest._  
_While either 32-bit (x86) or 64-bit (x86-64) versions should work just fine, I tend to gravitate to 32-bit installs as I have encountered other libraries/modules in the past that only offered 32-bit versions.  I have no idea if those modules that pushed me to 32-bit in the past still do not support 64-bit, but I'm a creature of habit._
* Verify a successful installation by opening a command prompt window and navigating to your Python installation directory (default is `C:\Python27`).  Type `python` from this location to launch the Python interpreter.
    ```
    Microsoft Windows [Version 6.2.9200]
    (c) 2012 Microsoft Corporation. All rights reserved.
    
    C:\Users\Username>cd C:\Python27
    
    C:\Python27>python
    Python 2.7.8 (default, Jun 30 2014, 16:03:49) [MSC v.1500 32 bit (Intel)] on win
    32
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    ```
* It would be nice to be able to run Python from any location without having to constantly reference the full installation path name.  This can by done by adding the Python installation path to Windows' `PATH` `ENVIRONMENT VARIABLE`  
*_In Windows 7 and Windows 8, simply searching for "environment variables" will present the option to `Edit the system environment variables`. This will open the `System Properties / Advanced` tab_  
*_In Windows XP, right click on `My Computer->Properties` to open `System Properties` and click on the `Advanced` tab._  
 1. On the `System Properties / Advanced` tab, click `Environment Variables` to open `User Variables` and `System Variables`
 2. Create a new `System Variable` named Variable name: `PYTHON_HOME` and  Variable value: `c:\Python27` (or whatever your installation path was)  
![](https://camo.githubusercontent.com/767e3e7294af750e7db47ffb119cdc1154e2c79f/68747470733a2f2f662e636c6f75642e6769746875622e636f6d2f6173736574732f323939363230352f313035383236332f38643062376334632d313138352d313165332d383532622d3863653063303263623464322e706e67)
 3. Find the system variable called `Path` and click `Edit`  
![](https://camo.githubusercontent.com/da06b60252e8293d278d2027544d23602daa853b/68747470733a2f2f662e636c6f75642e6769746875622e636f6d2f6173736574732f323939363230352f313035383239342f30643734343936382d313138362d313165332d383766302d6531326166323330353030612e706e67)
 4. Add the following text to the end of the Variable value:  `;%PYTHON_HOME%\;%PYTHON_HOME%\Scripts`
![](https://camo.githubusercontent.com/fb28d689631f2f4012741f6cf599dd52ed720b92/68747470733a2f2f662e636c6f75642e6769746875622e636f6d2f6173736574732f323939363230352f313035383237362f63333566353334612d313138352d313165332d386631622d6439343033633836643939662e706e67)
 5. Verify a successful environment variable update by opening a new command prompt window (important!) and typing `python` from any location
    ```
    Microsoft Windows [Version 6.2.9200]
    (c) 2012 Microsoft Corporation. All rights reserved.
    
    C:\Users\Username>python
    Python 2.7.8 (default, Jun 30 2014, 16:03:49) [MSC v.1500 32 bit (Intel)] on win
    32
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    ```

# Pip install
The easiest way to install the `matplotlib` and `numpy` python modules and keep them up-to-date is with a Python-based package manager called [Pip](http://en.wikipedia.org/wiki/Pip_(package_manager))

There are many methods for getting Pip installed, but my preferred method is the following:
* Download [get-pip.py](https://bootstrap.pypa.io/get-pip.py) to a folder on your computer. Open a command prompt window and navigate to the folder containing `get-pip.py`. Then run `python get-pip.py`. This will install `pip`.
* Verify a successful installation by opening a command prompt window and navigating to your Python installation's script directory (default is `C:\Python27\Scripts`).  Type `pip freeze` from this location to launch the Python interpreter.  
_`pip freeze` displays the version number of all modules installed in your Python non-standard library;  On a fresh install, `pip freeze` probably won't have much info to show but we're more interested in any errors that might pop up here than the actual content_
    ```
    Microsoft Windows [Version 6.2.9200]
    (c) 2012 Microsoft Corporation. All rights reserved.
    
    C:\Users\Username>cd c:\Python27\Scripts
    
    c:\Python27\Scripts>pip freeze
    antiorm==1.1.1
    enum34==1.0
    requests==2.3.0
    virtualenv==1.11.6
    ```
* It would be nice to be able to run Pip from any location without having to constantly reference the full installation path name.  If you followed the Python installation instructions above, then you've already got the pip install location (default = `C:\Python27\Scripts`) in your Windows' `PATH` `ENVIRONMENT VARIABLE`.  If you did not follow those steps, refer to them above now.
* Verify a successful environment variable update by opening a new command prompt window (important!) and typing `pip freeze` from any location
    ```
    Microsoft Windows [Version 6.2.9200]
    (c) 2012 Microsoft Corporation. All rights reserved.
    
    C:\Users\Username>pip freeze
    antiorm==1.1.1
    enum34==1.0
    requests==2.3.0
    virtualenv==1.11.6
    
# Linux Installation
 All linux distro's run python natively. Hence there is no need to install python separately. Just check if you pip installation is up to date.
 To update or install pip on Linux/Ubuntu just type in 
 - `sudo apt-get update && sudo apt-get install python-pip`
 
 
 
 # Installation of numpy and matplotlib
 Assuming you have a working installation of python and pip, installing these libraries is very easy.
 Just fire up a terminal and type in
 - `pip install matplotlib`
 - `pip install numpy`

# Pick and Install a Text Editor of choice
In case you have no idea what a text editor is or don't know which to pick, pick one from the list below
- Sublime Text
- Atom
- Brackets.io
- Vim

As for their installation, please visit their webistes.

###### NOTE: In case you get any errors while running the above commads, don't lose hope, just try and look up the error on google and try and fix it.
