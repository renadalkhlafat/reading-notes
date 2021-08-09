## API Design Best Practices

1. What does REST stand for?

`Representational State Transfer`

2. REST APIs are designed around a `resources`.

3. What is an identifer of a resource? Give an example.

`niquely identifies that resource ,ex (https://adventure-works.com/orders/1) `

4. What are the most common HTTP verbs?
   - GET 
   - POST 
   - PUT 
   - PATCH 
   - DELETE  

5. What should the URIs be based on?

`URI = scheme "://" authority "/" path [ "?" query ] [ "#" fragment ] `

6. Give an example of a good URI.

`example.com/articles/3252`

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?


`API that requires consumer to do more than a single call to perform a single, common operation `

8. What status code does a successful GET request return?

`200 `

9. What status code does an unsuccessful GET request return?

`404 `

10. What status code does a successful POST request return?

`201 `

11. What status code does a successful DELETE request return?

`204 `
