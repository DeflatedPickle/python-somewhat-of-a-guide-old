# Chapter 3.8: Classes {#classes}

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

```
class MyClass(object):
    pass
```

If no class is given to inherit, the class will inherit from `object`.

## Methods {#methods}

#### What is a Method? {#what-is-a-variable}

A method is what functions of a class are called. They are the same as normal functions, except they take an additional argument for the first parameter, the class.

#### How to Create an Method

```py
def my_method(self):
    pass
```

## Instances {#instances}

#### What is an Instance?

An instance of a class contains everything that the class has. The instance can use the class methods and variables, and can even have those variables contain different things.

#### How to Create an Instance

To create an instance, you simply type the name followed by an empty set of parentheses.

```py
MyClass()
```



