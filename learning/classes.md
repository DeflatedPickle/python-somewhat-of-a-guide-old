# Classes

## What is a Class?

A class is an object that can contain variables and methods. Multiple instances of the class can be created and used independent of eachother.

### Why Should I Use Classes?

## Using Classes

### How to Create a Class

The code below will create an empty class.

```python
class MyClass:
    pass
```

## Inheritance {#inheritance}

### What is Inheritance? {#what-is-inheritance}

Inheritance is when a class extends another, or multiple others.

When a class is extended by another, the new class will contain everything the extended class had.

### How to Inherit From a Class {#how-to-inherit-from-a-class}

To inherit from another class, simply type it's name inside a set of parentheses..

```python
class MyClass(object):
    pass
```

To inherit from multiple, simply place a comma after each class you would like to extend

```python
class MyClass(object, str):
    pass
```

If no class is given to inherit, the class will inherit from `object`.

## Class Initialiser {#class-constructor}

### What is the Class Initialiser? {#what-is-the-class-constructor}

The class initialiser is a method that is run whenever an instance of the class is created. It is where instance variables will be created.

```python
class MyClass:
    def __init__(self):
        self.name = "Monty"
```

### Initialiser Arguments {#constructor-arguments}

You might find that you want to pass arguments into the class for it to use. These arguments can be passed after `self`.

```python
class MyClass:
    def __init__(self, name):
        self.name = name
```

Now the name can be retrieved from an instance of the class.

### Running the Initialiser of an Extended Class {#running-the-constructor-of-an-extended-class}

If you extend from a class that sets variables in it's initialiser, you will notice that those variables will not be set in your extended class if you have an initialiser. This is because the extended class's constructor is never run. To fix this, you will need to run the initialiser inside yours.

```python
class MyClass(OtherClass):
    def __init__(self):
        OtherClass.__init__(self)
```

## Methods {#methods}

### What is a Method? {#what-is-a-method}

A method is what functions of a class are called. They are the same as normal functions, except they take an additional argument for the first parameter, the class.

### How to Create a Method {#how-to-create-a-method}

```python
def my_method(self):
    pass
```

## Class Variables {#class-variables}

### What is a Class Variable? {#what-is-a-class-variable}

A class variable is a variable that belongs to the class. In every instance of the class, class variables will always stay the same. They are defined before the constructor.

```python
class MyClass:
    my_variable = "Hello."
```

## Instance Variables {#instance-variables}

### What is an Instance Variable? {#what-is-an-instance-variable}

An instance variable is a variable of the class that can be used from an instance. They are defined in the constructor of the class.

```python
class MyClass:
    def __init__(self):
        self.my_variable = "Hello."
```

If the variable name lacks the `self.`, it will instead be a local variable.

## Instances {#instances}

### What is an Instance? {#what-is-an-instance}

An instance of a class contains everything that the class has. The instance can use the class methods and variables, and can even have those variables contain different things.

### How to Create an Instance {#how-to-create-an-instance}

To create an instance, you simply type the name followed by an empty set of parentheses.

```python
MyClass()
```

If the class takes arguments in the constructor, they will need to be given in the instance.

```python
MyClass("Monty")
```

