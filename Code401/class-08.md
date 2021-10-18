# List comprehension
 Is a powerful and concise method for creating lists and it is an elegant way to define and create lists based on existing lists

![list](https://www.freecodecamp.org/news/content/images/2021/07/list-comprehension-1.png)
## Syntax

```python
my_new_list = [ expression for item in list ]
```
![syntax](https://cdn.programiz.com/sites/tutorial2program/files/lc.jpg)

### Create a List with range()
```python
# construct a basic list using range() and list comprehensions
digits = [x for x in range(10)]

print(digits)
```
### Create a List Using Loops and List Comprehension in Python 
```python
# create a list using a for loop
squares = []

for x in range(10):
    # raise x to the power of 2
    squares.append(x**2)

print(squares)
```

### Multiplying Parts of a List

```python 
# create a list with list comprehensions
multiples_of_three = [ x*3 for x in range(10) ]

print(multiples_of_three)
```
### Show the first letter of each word using Python

```python
# a list of the names of popular authors
authors = ["Ernest Hemingway","Langston Hughes","Frank Herbert","Toni Morrison",
    "Emily Dickson","Stephen King"]

# create an acronym from the first letter of the author's names
letters = [ name[0] for name in authors ]
print(letters)
```

### Lower/Upper case converter using Python

```python
lower_case = [ letter.lower() for letter in ['A','B','C'] ]
upper_case = [ letter.upper() for letter in ['a','b','c'] ]

print(lower_case, upper_case)
```
### Print numbers only from a given string

```python
# user data entered as name and phone number
user_data = "Elvis Presley 987-654-3210"
phone_number = [ x for x in user_data if x.isdigit()]

print(phone_number)
```

