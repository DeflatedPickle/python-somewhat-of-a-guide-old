# Syntax Specifics

## Colons

Colons are used to specify a new block. They're placed at the end of function declarations, class declarations, if statements, for loops, etc.

```python
if 0 == 0:  # I've started a new block, the colon shows this
    pass
```

## Indentation

Python is an indentation based language. Indentation is very important to your code, and with out it, you'll be getting a few good errors.

### Why Did They Do This?

Python is supposed to be a language that is easy to use for beginners. This means that it must be easy to read, understand and write. In a few other languages, indentation doesn't matter whatsoever, and so code can become a lot harder to read.

When indentation is forced, like with Python, it makes code easier to read when skimming or looking through someone else's code.

### When Do I Indent?

Whenever you start a code block, which are started with a colon \("\`:\`"\), the next line will always be indented by one more indentation level. 

```python
var = "Hello"

if var == "Hello":
    print("It is!") # Indented 
```

The indentation level of this block must stay the same through out it, but not all blocks have to be indented to the same level:

```python
def function():
        pass  # Indented by 8 spaces - perfectly valid
        
def function():
    print("Hello, World!")
            pass  # Indented by 8 spaces - invalid, as the previous line is indented by 4
```

