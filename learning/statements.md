# Chapter 3.3: Statements {#statements}

#### What is a Statement? {#what-is-a-statement}

## Simple Statements {#simple-statements}

## Compound Statements {#compound-statements}

### If Statements

The `if` statement can be used to check if an argument is true or false.

For instance:

```py
if 0 == 0:
    print("Indeed.")
```

Will always be `true` and so print, "Indeed.", since 0 is always equal to 0.

#### In-Line

The `if` statement can be used in-line, to set a value to a piece of data depending on if the statement is true or false.

```py
print("Hello." if 0 == 0 else "Bye.")
```

### While Statement

The `while` statement will continue to run the code it contains until the argument it was given is not true.

```py
while True:
    print("Hello.")
```

This will always print, "Hello.", since `True` is always true.

