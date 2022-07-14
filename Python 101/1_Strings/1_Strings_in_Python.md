```python

my_string = "Welcome to Python!"
another_string = 'The bright red fox jumped the fence.'
a_long_string = '''This is a
multi-line string. It covers more than
one line'''

print(my_string)
print(another_string)
print(a_long_string)

```

The triple quoted line can be done with three single quotes or three double quotes. Either way, they allow the programmer to write strings over multiple lines.
If you print it out, you will notice that the output retains the line breaks.


```python
my_string = "I'm a Python programmer!"
otherString = 'The word "python" usually refers to a snake'
tripleString = """Here's another way to embed "quotes" in a string"""

print(my_string)
print(otherString)
print(tripleString)
```
The code above demonstrates how you could put single quotes or double quotes into a string.


```python
my_number = 123
my_string = str(my_number)

print(my_number)
print(my_string)
```

This is known as casting. You can cast some data types into other data types, like numbers into strings. But you’ll also find that you can’t always do the reverse, such as casting a string like ‘ABC’ into an integer.


```python
my_string = "abc"
my_string[0] = "d"
# TypeError: 'str' object does not support item assignment
```

It should be noted that a string is one of Python immutable types. What this means is that you cannot change a string’s content after creation.


```python
my_string = "abc"
print(id(my_string)) # 140029410169552

my_string = "def"
print(id(my_string)) # 140029409549312

my_string = my_string + "ghi"
print(id(my_string)) # 140029409549200
```

By checking the id of the object, we can determine that any time we assign a new value to the variable, its identity changes.

The ‘+’ operator concatenates the two strings into one.


```python
my_unicode_string = u"This is unicode!"
```
The example above doesn’t actually contain any unicode, but it should give you the general idea. In Python 3.x, all strings are unicode.
