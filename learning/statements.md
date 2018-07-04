# Statements

## What is a Statement?

### Why Should I Use Statements?

## Simple Statements {#simple-statements}

## Compound Statements {#compound-statements}

### If Statements

The `if` statement can be used to check if an expression is true or false.

With this `if` statement, I check the equality of 0 against 0.

```python
if 0 == 0:
    print("Indeed")
```

Will always be true and so print, "Indeed", since 0 is always equal to 0.

Equality is checked on a type basis, as well as on an instance basis. So this `if` statement, will not run the code inside, as it's comparing an integer and a string.

```python
if 0 == "0":
    print("It's not")
```

#### Else

If you want to run some code when the argument is false, you can use `else`.

```python
if 0 == "0":
    print("Indeed")
else:
    print("I should think not")
```

#### Elif

If you want to check something else if the argument is false, you can use an `elif`. An `elif` means, "else if".

```python
if 0 == 1:
    print("Indeed")
elif 0 == 0:
    print("It does")
else:
    print("I should think not")
```

#### In-Line

The if statement can be used in-line, to set a value to a piece of data depending on if the statement is true or false.

```python
print("Hello" if 0 == 0 else "Bye")
```

### While Statement

The while statement will continue to run the code it contains until the expression it was given is not true.

```python
while 0 == 0:
    print("Hello")
```

This will print, "Hello" until the program is closed, since 0 always equals 0.

If you want your program to loop forever, it is best to use `while True`, as it provides good readability.

If you would like your program to loop until a variable is changed, you can use `while my_variable`, after setting the variable to `True`, first. This will then run forever, or until you reset the variable to something else. If it is set to something else, the `while` loop will exit after the rest of the code inside has finished.

```python
my_variable = True
counter = 0

while my_variable:
    print("Hello")
    counter += 1
    
    if counter > 10:
        my_variable = False
```

