## Loops

- refer to this link also

https://github.com/its-sachink/my_python_notes/blob/master/Python_Basic/1_Revision.md


#### The 'for' loop

- Sample python codes for looping

```python
print(range(5))  # range(0, 5)

print(range(5,10))  # range(5, 10)
print(list(range(1, 10, 2)))  # [1, 3, 5, 7, 9]


for number in range(5):
    print(number)

# 0
# 1
# 2
# 3
# 4

for number in [0, 1, 2, 3, 4]:
    print(number)



>>> a_dict = {"one":1, "two":2, "three":3}
>>> for key in a_dict:
       print(key)

three
two
one





a_dict = {1:"one", 2:"two", 3:"three"}
keys = a_dict.keys()
keys = sorted(keys)
for key in keys:
    print(key)

# 1
# 2
# 3




for number in range(10):
    if number % 2 == 0:
        print(number)
# 0
# 2
# 4
# 6
# 8
```



#### The 'while' loop

```python

i = 0
while i < 10:
    print(i)
    if i == 5:
        break
    i += 1

# 0
# 1
# 2
# 3
# 4
# 5
```

The break builtin is known as a flow control tool. There is another one called **continue** that is used to basically skip an iteration or continue with the next iteration.


```python

i = 0

while i < 10:
    if i == 3:
        i += 1
        continue

    print(i)

    if i == 5:
        break
    i += 1

```

Basically we added a second conditional that checks if i equals 3. If it does, we increment the variable and continue with the next loop, which effectively skips printing the value 3 to the screen. As before, when we reach a value of 5, we break out of the loop.


