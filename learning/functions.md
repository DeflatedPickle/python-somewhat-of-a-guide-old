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
```

```py
def greet_long(first_name, second_name):
    print("Hello, " + first_name + " " + second_name + "!")
```

This will print, "Hello, Monty Python!".

#### Default Value

By default, the values of arguments are all empty, and so every one must have a value past to it. However, you might want to give default values for arguments. This can be done by adding an equals sign and then the value, just like you were creating a variable.

```py
def greet(name="Monty"):
    print("Hello, " + name + "!")
```

#### Passing Arguments

To pass values to function arguments, you will need to add the data to the set of parentheses.

```py
greet("Monty")
```

If there are multiple arguments for a function, to set their values, you will need to set them in the order they come in the function.

You can also pass the name of the argument and then it's value.

```py
greet(name="Monty")
```

Passing them with the name means that you can give the values anywhere in the parentheses.

```py
greet_long(second_name="Python", first_name="Monty")
```

These aren't an either/or situation, though. Both can be used together.

```py
greet_long("Monty", second_name="Python")
```

Using the name of the argument will improve readability of the code, and if you think someone else will need to understand what the arguments mean, it might be a good idea to use them.

#### What are Args and Kwargs?

## Returning Information {#returning-information}

Functions can return information to be used elsewhere.

```py
def sum(num1, num2):
    return num1 + num2

print(sum(1, 2))
```

This function will add the 2 arguments together.

## Coroutines {#coroutines}

#### What is a Coroutine?



