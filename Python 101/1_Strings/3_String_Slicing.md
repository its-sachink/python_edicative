Each character in a string can be accessed using slicing. For example, if I want to grab just the first character, I could do this:

```python
my_string = "I like Python!"
print(my_string[0:1])

my_string = "I like Python!"

print(my_string[:1])   # 'I'
print(my_string[0:12]) # 'I like Pytho'
print(my_string[0:13]) # 'I like Python'
print(my_string[0:14]) # 'I like Python!'
print(my_string[0:-5]) # 'I like Py'
print(my_string[:])    # 'I like Python!'
print(my_string[2:])   # 'like Python!'  
```

You can also access individual characters in a string via indexing. Here is an example:

```python
my_string = "I like Python!"
print(my_string[0])
print(my_string[2])
print(my_string[7]) 
print(my_string[100]) # IndexError: string index out of range
```
