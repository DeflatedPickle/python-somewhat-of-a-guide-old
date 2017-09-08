# Chapter 2.2: Type Hinting {#statements}

#### What is Type Hinting?

Type hinting is where you specify the class type that a variable will be, for instance, `str`.

This is mostly for documentation, though it will help with readability and understanding of the code.

## Argument Type

To specify the type of an argument, add a colon after the name and then the class type.

```py
def greet(name: str):
    print("Hello, " + name + "!")

greet("Monty")
```

## Return Type

The type of the returned value can be specified by adding an arrow after the function, followed by the class type and then the colon.

```py
def sum(num1, num2) -> int:
    return num1 + num2

print(sum(1, 2))
```



