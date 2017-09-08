# Chapter 3.9: Classes {#classes}

#### What is a Class? {#what-is-a-variable}

A class is an object that can contain variables and methods. Multiple instances of the class can be created and used independent of eachother.

#### How to Create a Class

The code below will create an empty class.

```py
class MyClass:
    pass
```

## Inheritance {#inheritance}

#### What is Inheritance? {#what-is-a-variable}

Inheritance is when a class extends another, or multiple others.

When a class is extended by another, the new class will contain everything the extended class had.

#### How to Inherit From a Class

To inherit from another class, simply type it's name inside a set of parentheses.

```py
class MyClass(object):
    pass
```

If no class is given to inherit, the class will inherit from `object`.

#### Class Constructor

#### What is the Class Constructor? {#what-is-a-variable}

The class constructor is a method that is run whenever an instance of the class is created. It is where instance variables will be created.

```py
class MyClass:
    def __init__(self)
        pass
```

## Methods {#methods}

#### What is a Method? {#what-is-a-variable}

A method is what functions of a class are called. They are the same as normal functions, except they take an additional argument for the first parameter, the class.

#### How to Create an Method

```py
def my_method(self):
    pass
```

## Class Variables {#instances}

#### What is a Class Variable?

A class variable is a variable that belongs to the class. In every instance of the class, class variables will always stay the same. They are defined before the constructor.

```py
class MyClass:
    my_variable = "Hello."
```

## Instance Variables {#instances}

#### What is an Instance Variable?

An instance variable is a variable of the class that can be used from an instance. They are defined in the constructor of the class.

```py
self.my_variable = "Hello."
```

## Instances {#instances}

#### What is an Instance?

An instance of a class contains everything that the class has. The instance can use the class methods and variables, and can even have those variables contain different things.

#### How to Create an Instance

To create an instance, you simply type the name followed by an empty set of parentheses.

```py
MyClass()
```



