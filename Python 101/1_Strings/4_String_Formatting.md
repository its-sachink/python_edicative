#### Old Way of Substituting Strings.

```python
my_string = "I like %s" % "Python"
print(my_string) # 'I like Python'

var = "cookies"
newString = "I like %s" % var
print(newString) # 'I like cookies'

another_string = "I like %s and %s" % ("Python", var)
print(another_string)  # 'I like Python and cookies'
```


If we don’t insert enough strings:

```python
another_string = "I like %s and %s" % "Python"

print(another_string)
# TypeError: not enough arguments for format string
```


How to insert integers and floats

```python
my_string = "%i + %i = %i" % (1,2,3)
print(my_string) # '1 + 2 = 3'

float_string = "%f" % (1.23)
print(float_string) # '1.230000'

float_string2 = "%.2f" % (1.23)
print(float_string2) # '1.23'

float_string3 = "%.2f" % (1.237)
print(float_string3) # '1.24'
```

check out for errors
```python
int_float_err = "%i + %f" % ("1", "2.00")
print(int_float_err)
# TypeError: %i format: a number is required, not str

int_float_err = "%i + %f" % (1, "2.00")
print(int_float_err)
# TypeError: a float is required


int_float_str = "%i + %f" % (1, 2.00)
print(int_float_str)
# 1 + 2.000000
```

#### New way of substituing the strings

```python
print("%(lang)s is fun!" % {"lang":"Python"})
# Python is fun!

print("%(value)s %(value)s %(value)s !" % {"value":"SPAM"})
# SPAM SPAM SPAM !

print("%(x)i + %(y)i = %(z)i" % {"x":1, "y":2})
# KeyError: 'z'

print("%(x)i + %(y)i = %(z)i" % {"x":1, "y":2, "z":3})
# 1 + 2 = 3
```

###### We can also use the format in the string

```python
print("Python is as simple as {0}, {1}, {2}".format("a", "b", "c"))
# 'Python is as simple as a, b, c'

print("Python is as simple as {1}, {0}, {2}".format("a", "b", "c"))
# 'Python is as simple as b, a, c'

xy = {"x":0, "y":10}
print("Graph a point at where x={x} and y={y}".format(**xy))
# Graph a point at where x=0 and y=10
```
