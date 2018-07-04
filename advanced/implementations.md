# Implementations

Python, being a language favored by many, has quite a few different implementations. An implementation being a form of Python that is run in a different way and/or written in a different languages. Examples of different implementations consist of Jython, which runs on the JVM and can interact with Java code and IronPython, which runs on .NET and can interact with C\# code. These other implementations are not official and can sometimes be for older versions, as they usually have small teams working on them. The main and official implementation of Python is CPython.

## [PyPy](https://pypy.org/)

PyPy is an alternative implementation of Python 3 and Python 2, written in Python, that features a JIT compiler. This makes PyPy usually run faster than the official implementation, meaning it's great for work that Python would usually slow down on.

## [Jython](https://hg.python.org/jython)

Jython is an implementation of Python 2 that runs on the JVM. It's usually faster than the official implementation, as it runs on the JVM. It can easily import Java code, the same way you'd import Python code. Unfortunately, there's no Jython for Python 3.

## [IronPython](http://ironpython.net/)

IronPython is an implementation of Python 2 that runs on .NET. Like Jython, it's usually faster than the official implementation as it's compiled to and then run on a virtual machine, in this case, the CLR \(Common Language Runtime\), rather than interpreted \(like the official implementation\). They way IronPython differs from Jython is that it interacts with .NET rather than the JVM, so instead of being able to import Java code, you can import C\# code and Python code. But again, like Jython, there's no implementation for Python 3.

