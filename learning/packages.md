# Packages

A package is a collection of variables, functions and classes for you to use, usually written by someone else or included with Python, though you are able to easily write your own packages and distribute them for others to download and use.

## Importing Packages {#importing-packages}

A package can be imported with the import statement.

```python
import math
```

This will import the "math" library, which includes functions for different math related tasks, such as the "floor" function, which will return the number given, rounded down. To use this function, we need to first specify the package name and then access the function from it, with a period.

```python
print(math.floor(5.5))
```

This will then print "5".

Though if you need to use this function multiple times, and don't want to type out the package name each time, you can import everything from the library into the local namespace, like so:

```python
from math import *
```

Though if you import multiple libraries that each have a function named the same thing, the function available will be the last library imported, though you can bind the function from the first imported library to a new name first, then import the second library.

If you instead want to import just one or a few things from the library into the local namespace instead of importing it all or importing the package, you can replace the asterisks from the last example with the variable, function or class name, for one thing, or the every name, with a comma between each name.

```python
from math import floor  # Imports floor from math

from math import floor, ceil  # Imports floor and ceil from math
```

Now, I can use the function "floor" by just specifying the function name:

```python
print(floor(5.5))
```

For a full list of packages included with Python, and the variables, functions and classes in them, visit the [Python library reference](https://docs.python.org/3/library/).

## Installing Packages {#installing-packages}

Python has a specific site for packages to be hosted on and downloaded from, called [PyPI](https://pypi.org/) \(the Python Package Index\). This site can be used to find new packages, locate packages you know of, and read and find links on each package.

To install a package from PyPI, first make sure that Python is in your system PATH, and then in the terminal for your OS, write "`pip install`" and then the package name. 

To upgrade an already installed package, again write "`pip install`" followed by the package name but then add the `--upgrade` flag.

## Creating Packages {#creating-packages}

To create a Python package, you will first need to create a directory, then inside of the directory, you will need to create a file named `__init__.py` , this is the initialization file. After that, you're free to add the scripts you want to the directory, but to include them in the package, you will need to import them in the initialization file, unless you want for your user to need to type the package name and then the file name, this is usually what package authors do with submodules.

Submodules are basically a Python package inside of a Python package, and are used to section off scripts, both to make navigating the package easier, but also to keep the user from importing potentially hundreds of functions.

### Uploading A Package To PyPI

To upload your package to PyPI, you will need to first create a file named `setup.py` in the same directory as your package, then import `setup` from `setuptools`, and then call the `setup` function.

```python
from setuptools import setup

setup(name="package",
      version="1.0.0",
      description="My package.",
      author="Me",
      classifiers=[
          "Intended Audience :: Developers",
          "Programming Language :: Python :: 3.6",
      ],
      keywords=["package"],
      packages=["package"])
```

The `setup` function takes quite a few arguments for your package, most being optional. The most necessary arguments are `name`, `version` and `packages`. The name being the name of your package, the version being the version of this release, and packages being the packages included in this release, this will most likely just be the name of your package folder. Though if your package includes submodules, you will also need to specify them in the packages argument.

After that's done, you'll then need to install [Twine](https://github.com/pypa/twine) through PIP, then open a terminal instance in the directory containing your package folder and the `setup.py` file and run `python setup.py sdist` to create a release of your package, and then run  `twine upload dist/*` to upload your package to PyPI. You'll be prompted to enter your username and password, which bare in mind, won't move the text carat or appear as stars, and then your package will appear on PyPI. It will take a few minutes to sync, and then you'll be able to install your package with PIP.

