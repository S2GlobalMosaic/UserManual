# UserManual
In this repository the  user manual for S2 Global Mosaic is stored and maintained.
This readme gathers all the necessary bits and pieces which are good to know when working on this documentation, 
e.g. on how the project must be set up in order to build it locally and which formatting rules to obey.

## Local Python & Sphinx Setup
See [Getting Started Guide](https://docs.readthedocs.io/en/latest/getting_started.html)
 
### Building the documentation locally
* It is best to build the documentation locally on a unix system. If you are on Windows you can use 
the [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10) and install e.g an 
Ubuntu version.
* After you have initialised the system and installed sphinx and other necessary tools and have setup the project 
(see [Getting Started Guide](https://docs.readthedocs.io/en/latest/getting_started.html)) you can switch to the 
project directory on the console.
* In order to create HTML page invoke:

```
$ make html
```
     
This creates the HTML pages and the static directory structure for the documentation.

## Editing

### reST Format Documentation
The basic formatting rules for reST documents can be found here: [sphinx-doc.org](http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)

 
