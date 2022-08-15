## Comprehensions

- Refer to this link

https://github.com/its-sachink/my_python_notes/blob/master/Python_Basic/2_Revision.md


#### List comprehensions

- Sample examples

```python
x = [i for i in range(5)]
print(x)

--
if [i for i in line if "SOME TERM" in i]:
    # do something


--
x = ['1', '2', '3', '4', '5']
y = [int(i) for i in x]
print(y) # [1, 2, 3, 4, 5]


--
myStringList = [
  '    Hello how are you?',
  'I\'m good    ',
  '    I\'m good too   ']
myStrings = [s.strip() for s in myStringList]
print(myStrings)
---- output ----
['Hello how are you?', "I'm good", "I'm good too"]




--
vec = [[1,2,3], [4,5,6], [7,8,9]]
flatVec = [num for elem in vec for num in elem]
print(flatVec) # [1, 2, 3, 4, 5, 6, 7, 8, 9]
---- output ----
[1, 2, 3, 4, 5, 6, 7, 8, 9]
```


#### Dictionary comprehensions

- Sample examples

```python

print( {i: str(i) for i in range(5)} )
# {0: '0', 1: '1', 2: '2', 3: '3', 4: '4'}



my_dict = {1:"dog", 2:"cat", 3:"hamster"}
print( {value:key for key, value in my_dict.items()} )
# {'hamster': 3, 'dog': 1, 'cat': 2}

```

#### Set comprehensions

- Sample examples


```python
my_list = [1, 2, 2, 3, 4, 5, 5, 7, 8]
my_set = set(my_list)
print(my_set)
# {1, 2, 3, 4, 5, 7, 8}


my_list = [1, 2, 2, 3, 4, 5, 5, 7, 8]
my_set = {x for x in my_list}
print(my_set)
# {1, 2, 3, 4, 5, 7, 8}

```