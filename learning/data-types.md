# Chapter 3.1: Data Types {#data-types}

Text

### None

None is litterly nothing. No data, No value, no nothing

## Numeric {#numeric}

A numberic data type contains a number, like 1942302. For example

```python
PI = 3
```

PI will now contain the number 3 which can now be used in calculating stuff

### Boolean {#boolean}

A boolean can be in 2 states, true or false.
A boolean can be the answer to a question or statement,
for example:

```python
is_user_bot = true
```

IsUserBot now contains True which means the User is a bot

Booleans are mostly used in if, while, for, etc loops, these loops will only run if the value is true

```python
if(is_user_bot):
  print("User is a bot!")
```

will print "User is a bot!" if IsUserBot is true

### Float {#float}

Float is like a numeric number as explained above but it has decimals, for example if you wanted more specific calculations you can do

```python
PI = 3.14
```

PI now contains the more correct 3.14 instead of just a 3

### Complex {#complex}

Explaining complex numbers

## Sequences {#sequences}

Something about sequences

### String {#string}

Strings are just text, like what you're reading right now. You define a string by putting your text around quotation marks, for example

```python
my_name = "deflatedpickle"
print(my_name)
```

this will print "deflatedpickle"(without the quotation marks)

### Bytes {#bytes}

a computer stores data in bits as you may know, 1s and 0s.

A byte is 8 bits, for example 01100011 is a byte because it contains 8 bits, This byte is the number 99. Here's a quick tutorial on how to read bytes/bits, known as binary. https://www.wikihow.com/Read-Binary

### Byte Array {#byte-array}

A byte array is an array of bytes(explained above)

### List {#list}

Explaining lists

### Array {#array}

Explaining arrays

### Tuple {#tuple}

Explaining tuples

## Sets {#sets}

Something about sets

### Set {#set}

Explaining sets

### Frozen Set {#frozen-set}

Explaining frozen sets

## Mappings {#mappings}

Something about mappings

### Dictionary {#dictionarie}

Dictionarys are kind of like arrays but instead of accessing them with a number index, you can use any other type of data. For example

```python
dict = { 'Username': 'XXEliteMaster64XX', 'Level': 10 } ##Creates a dictionary with a key named "Username" containing "XXEliteMaster64XX" and another key named "Level" containing 10
player_username = dict['Username'] ##Getting the username by accessing the dictionary with a key of "Username"
print(player_username)
```

this will print "XXEliteMaster64XX" because the dictionary key "Username" contains the value "XXEliteMaster64XX"
