# Dunder Methods or Magic methods
 Are the methods having two prefix and suffix underscores in the method name

## Object Initialization: `__init__ `
The `__init__` method for initialization is invoked without any call, when an instance of a class is created, like constructors in certain other programming languages

```python
class Account:
    """A simple account class"""

    def __init__(self, owner, amount=0):
        """
        This is the constructor that lets us create
        objects from this class
        """
        self.owner = owner
        self.amount = amount
        self._transactions = []
```
## Object Representation: `__str__`,` __repr__`

1. `__repr__`: The “official” string representation of an object. This is how you would make an object of the class. The goal of` __repr__` is to be unambiguous.

2. `__str__`: The “informal” or nicely printable string representation of an object. This is for the enduser.

```python
class Account:

    def __repr__(self):
        return 'Account({!r}, {!r})'.format(self.owner, self.amount)

    def __str__(self):
        return 'Account of {} with starting amount: {}'.format(
            self.owner, self.amount)
```

## Iteration: `__len__`, `__getitem__`, `__reversed__`

```python
class Account:
    # ... (see above)

    def __len__(self):
        return len(self._transactions)

    def __getitem__(self, position):
        return self._transactions[position]
    
    def __reversed__(self):
    return self[::-1]
```

## Callable Python Objects: `__call__`
we can make an object callable like a regular function by adding the `__call__` dunder method

```python
class Account:
    # ... (see above)

    def __call__(self):
        print('Start amount: {}'.format(self.amount))
        print('Transactions: ')
        for transaction in self:
            print(transaction)
        print('\nBalance: {}'.format(self.balance))
```

## Operator Overloading for Comparing Accounts: `__eq__`, `__lt__`

```python
from functools import total_ordering

@total_ordering
class Account:
    # ... (see above)

    def __eq__(self, other):
        return self.balance == other.balance

    def __lt__(self, other):
        return self.balance < other.balance
```

# Operator Overloading for Merging Accounts: `__add__`

```python
def __add__(self, other):
    owner = self.owner + other.owner
    start_amount = self.balance + other.balance
    return Account(owner, start_amount)
```
## Statistics - Probability
An event is some outcome of interest, we also need to consider all the other events that can occur.

![statesic](https://i.imgur.com/GtbawRt.jpg)
