# Statements

#### What is a Statement? {#what-is-a-statement}

## Simple Statements {#simple-statements}

## Compound Statements {#compound-statements}

### If Statements

The `if` statement can be used to check if an argument is true or false.

For instance:

```python
if 0 == 0:
    print("Indeed.")
```

Will always be `true` and so print, "Indeed.", since 0 is always equal to 0.

#### Else

If you want to run some code when the argument is false, you can use `else`.

```python
if 0 == 0:
    print("Indeed.")
else:
    print("I should think not.")
```

#### Elif

If you want to check something else if the argument is false, you can use an `elif`. An `elif` basically means, "else if".

```python
if 0 == 1:
    print("Indeed.")
elif 0 == 0:
    print("It does.")
else:
    print("I should think not.")
```

It can be substituted by placing another `if` statement inside an `else`, though this can decrease readability of the code.

```python
if 0 == 1:
    print("Indeed.")
else:
    if 0 == 0:
        print("It does.")
    else:
        print("I should think not.")
```

#### In-Line

The `if` statement can be used in-line, to set a value to a piece of data depending on if the statement is true or false.

```python
print("Hello." if 0 == 0 else "Bye.")
```

### While Statement

The `while` statement will continue to run the code it contains until the argument it was given is not true.

```python
while 0 == 0:
    print("Hello.")
```

This will print, "Hello." until the program is closed, since 0 always equals 0.

If you want your program to loop forever, it is best to use `while True`, as it provides good readability.

If you would like your program to loop until a variable is changed, you can use `while my_variable`, after setting the variable to `True`, first. This will then run forever, or until you reset the variable to something else. If it is set to something else, the `while` loop will exit after the rest of the code inside has finished.

