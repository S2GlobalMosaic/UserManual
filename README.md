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

### Versioning
The file `conf.py` contains two version properties. The one is called `version` and the is `release`
The version property should only contain the version number:
```
# The short X.Y version
version = '0.4'
```

The release property should also contain some tag indicating for example that the version is still in development.

```
# The full version, including alpha/beta/rc tags
release = '0.4-DEV'
```

If a release of the manual shall be done. Both version shall be the same and the GitHub repository shall be tagged with 
this version.

Afterwards check the setting in the readthedocs project if the versions are correctly accessible

## Editing

### reST Format Documentation
The basic formatting rules for reST documents can be found here: [sphinx-doc.org](http://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html)

 
