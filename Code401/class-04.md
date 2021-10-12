# Classes and Objects
**Class** : template to create an object that encapsulate variables and functions inside it and get them from the that class and we can access the variable and function by the object from the class using (.)

**Example** 
```python 
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

```
# Thinking Recursively
 The essence of thinking recursively is to break the problem down into small pecies to solve 

 ## Recursive Functions 
  A routine that calls itself directly or indirectly.

  **Example**
  ```python
  def fibonacci(n):
    if n <= 1:
        return n
    else:
        return fibonacci(n-1) + fibonacci(n-2)
  ```
## Recursive Data Structures 
 A data structure that is partially composed of smaller or simpler instances of the same data structure

**Eaxmple**
```python
def list_sum_recursive(input_list):
    # Base case
    if input_list == []:
        return 0

    # Recursive case
    # Decompose the original problem into simpler instances of the same problem
    # by making use of the fact that the input is a recursive data structure
    # and can be deﬁned in terms of a smaller version of itself
    else:
        head = input_list[0]
        smaller_list = input_list[1:]
        return head + list_sum_recursive(smaller_list)
```


# Fixtures and Coverage
 
**Fixtuers** : Fixtures are a set of resources that have to be set up before and cleaned up once the  test automation execution is completed ,and  we define fixtures using a combination of the `pytest.fixture` decorator, along with a function definition

**Example**
```python
@pytest.fixture
def simple_file():
   return StringIO('\n'.join(['abc', 'def', 'ghi', 'jkl']))

```

**Coverage**: a metric for how much of your codebase gets executed when you run your tests. Basically, it tells us how much of your code is covered by tests and, more important, helps you locate lines in your code that aren't covered