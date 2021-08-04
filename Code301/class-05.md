## React Docs - thinking in React

1. How would you break a mock into a component heirarchy?
 
`by drawing boxes around every component and subcomponent in the mock and give them all names `

2. What is the single responsibility principle and how does it apply to components?

`SRP, a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part`

3. What does it mean to build a ‘static’ version of your application?

` don’t use state at all `

4. Once you have a static application, what do you need to add?

`responsibility`

5. What are the three questions you can ask to determine if something is state?

`1. Is it passed in from a parent via props?`

`2. Does it remain unchanged over time? `

`3. Can you compute it based on any other state or props in your component?`



6. How can you identify where state needs to live?

``` 
Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state. 

```