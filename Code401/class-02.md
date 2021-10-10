## Unit tests
a pieces of code to check the input,the output and how the code work , basicly to test an algorithm how it's work 

## TDD
it stand or Test-Driven Development ,and it is a strategy to think and write the code and  When we are writing tests we are forced to think about the design first and how we can break it into small pieces.

## Important aspects about the unit test
 +  **Test name** : The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.

 + **The test file name**  should follow the same name of module name. __For instance__, if our module is `gender.py`, our test name should be `test_gender.py`

 ## AAA: Arrange, Act and Assert.
 + Arrange: (input)we need to organize the data needed to execute that piece of code .
+ Act: (exercise the behaviour) here we will execute the code being tested .
+ Assert:(output)  after executing the code, you will check if the result is the same as you were expecting.


 ```
 if __name__ == “__main__”: do?
```

If the python interpreter is running that module (the source file) as the main program, it sets the special `__name__` varable to have a value `__main__`. If this file is being imported from another module, `__name__` will be set to the module’s name. Module’s name is available as value to `__name__ `global variable. 

## Recursion
The process in which a function calls itself directly or indirectly 

**Example**
```
int fact(int n)
{
    if (n < = 1) // base case
        return 1;
    else    
        return n*fact(n-1);    
}
```