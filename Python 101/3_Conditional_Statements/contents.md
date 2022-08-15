## Checking for Nothing

There is also another keyword that basically evaluates to False which is called **None**. The None value is used to represent the absence of value. It’s kind of analogous to Null, which you find in databases.

```python
empty_list = []
empty_tuple = ()
empty_string = ""
nothing = None

if empty_list == []:
    print("It's an empty list!")

if empty_tuple:
    print("It's not an empty tuple!")

if not empty_string:
    print("This is an empty string!")

if not nothing:
    print("Then it's nothing!")

----- output -----
It's an empty list!
This is an empty string!
Then it's nothing!
```

The second conditional only evaluates to True if the tuple is not empty! The last two conditionals are doing the opposite of the second. The third is checking if the string is empty and the fourth is checking if the nothing variable is really None.



```python
empty_string = ""

if empty_string == "":
    print("This is an empty string!")

------ output ------
This is an empty string!
```

Please note that none of these variables equals the other.

```python
empty_list = []
empty_string = "something"
nothing = None

print(empty_list == empty_string) # False
print(empty_string == nothing) # False
```



## Special Characters :

```python
print("I have a \n new line in the middle")
print("This sentence is \ttabbed!")

------ output ------
I have a 
 new line in the middle
This sentence is 	tabbed!
```

In the case of a backslash, you would actually type two backslashes. Let’s take a look :

```python
print("This is a backslash \\")

------ output ------
This is a backslash \
```



## if __name__ == “__main__”

Does your Python program always starts at the top of the file or can you tell Python where to start?

You will see a very common conditional statement used in many Python examples.

```python
if __name__ == "__main__":
    # do something!

```

You will see this **at the end of a file**. This tells Python that you only want to **run the following code if this program is executed as a standalone file**.

We will be discussing this later in the course, but whenever you create a Python script, you create a Python module. If you write it well, **you might want to import it into another module**. When you do import a module, **it will not run the code that’s under the conditional because __name__ will no longer equal "__main__"**. 

