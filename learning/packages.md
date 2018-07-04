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

## Standard Packages {#standard-packages}

Stuff.

## Installing Packages {#installing-packages}

Many popular packages are available on pip, python's package manager. It is included with all python versions >= 2.7.9.

It can be used by typing "python -m pip install \[modulename\]", where modulename is the name of the module you want to install, in the terminal or command prompt, depending on which system you're on.

You can, of course, also uninstall packages you installed via pip. The command for that is "python -m pip uninstall \[modulename\]".



There are of course packages that are not available on pip, those can be installed either by using a third-party package manager / installer if one is available or by just downloading the .py file and putting it in your scripts folder.

## Creating Packages {#creating-packages}

Stuff.

