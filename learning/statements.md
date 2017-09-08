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

If you want to run some code when the argument is false, you can use `else`.

```py
if 0 == 0:
    print("Indeed.")
else:
    print("I should think not.")
```

#### In-Line

The `if` statement can be used in-line, to set a value to a piece of data depending on if the statement is true or false.

```py
print("Hello." if 0 == 0 else "Bye.")
```

### While Statement

The `while` statement will continue to run the code it contains until the argument it was given is not true.

```py
while 0 == 0:
    print("Hello.")
```

This will print, "Hello." until the program is closed, since 0 always equals 0.

