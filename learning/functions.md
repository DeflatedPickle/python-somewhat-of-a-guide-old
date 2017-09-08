# Chapter 3.8: Functions {#functions}

#### What is a Function?

A function is a command that can be used to perform an/or multiple actions. They can contain however many lines of code you would like, and can be used however many times by just calling it.

#### Why Should I Use Functions? {#why-should-i-use-variables}

Using functions will decrease the the amount of coding needed.

If you want to run multiple lines of code multiple times, then putting that code into a function will reduce the lines needed to 1. It also means that you can update the code run easily.

## Arguments {#arguments}

#### What is an Argument?

An argument is something that can be passed into a function to then be used inside of the function.

```py
def greet(name):
    print("Hello, " + name + "!")

greet("Monty")
```

This function will print, "Hello, Monty!". Since we passed the string, "Monty" into the function.

If there are multiple arguments for a function, to set their values, you will need to set them in the order they come in the function.

```py
def greet_long(first_name, second_name):
    print("Hello, " + first_name + " " + second_name + "!")

greet_long("Monty", "Python")
```

This will print, "Hello, Monty Python!".

#### What are Args and Kwargs?

### Type Hinting {#type-hinting}

#### What is Type Hinting?

Type hinting is where you specify the type that a variable will be.

This is mostly for documentation.

```py
def greet(name: str):
    print("Hello, " + name + "!")

greet("Monty")
```

## Returning Information {#returning-information}

Functions can return information to be used elsewhere.

```py
def sum(num1, num2):
    return num1 + num2

print(sum(1, 2))
```

This function will add the 2 arguments together.

### Return Type {#return-type}

## Coroutines {#coroutines}

#### What is a Coroutine?



