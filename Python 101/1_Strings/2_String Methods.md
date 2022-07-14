A string is an object in Python. In fact, everything in Python is an object.
strings have their very own methods built into them. For example, let’s say you have the following string:

```python
my_string = "This is a string!"
print(my_string.upper())

# Or more concisely
print("This is a string!".upper())
print("This is a string!".lower())
```

To get a list of all the string methods, you can use Python’s built-in function dir. Let’s look at this in action.

```python
my_string = "This is a string!"
print(dir(my_string))

# [
#   '__add__', '__class__', '__contains__', '__delattr__', 
#   ...
#   ...
#   ...
#  'translate', 'upper', 'zfill'
# ]
```

String is a object class in python

```python
my_string = "This is a string!"
print(type(my_string)) # <class 'str'>
```