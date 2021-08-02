## React Docs - lists and keys

1. What does .map() return?
` map object`
2. If I want to loop through an array and display each value in JSX, how do I do that in React?
`using map function to return a map object of the results after applying a given function to each item of a given iterable Parameters`
3. Each list item needs a unique `key`
4. What is the purpose of a key?
`to identify which items in the list are changed, updated or delete`

## The Spread Operator
1. What is the spread operator?
`an operator allows an iterable to expand in places where 0+ arguments are expected. `

2. List 4 things that the spread operator can do.

`Copying an array,Adding an item to a list, Combining objects,Using Math functions`

3. Give an example of using the spread operator to combine two arrays.

`let arr1 = ['a','b','c']; `

`let arr2 = ['d','e','e'];`

`let arr3 = [...arr1, ...arr2] `

4. Give an example of using the spread operator to add a new item to an array.

`let a = [1, 2, 3, 4, 5];` 

`let b = [0, ...a];`

5. Give an example of using the spread operator to combine two objects into one.

``` 
let person = {
    firstName: 'John',
    lastName: 'Doe',
};


let job = {
    jobTitle: 'JavaScript Developer',
};

let employee = {
    ...person,
    ...job
};
```
## How to Pass Functions Between Components
1. In the video, what is the first step that the developer does to pass functions between components?

`create the function that we want to pass it `

2. In your own words, what does the increment function do?

`increment the count property 1 when it called`

3. How can you pass a method from a parent component into a child component?

`by passing the name of the function `

4. How does the child component invoke a method that was passed to it from a parent component?

`using this.props.nameOfTheFunction `