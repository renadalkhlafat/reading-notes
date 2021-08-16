## Status Codes Based On REST Methods

- In your own words, describe what each group of status code represents:
100’s = `tell the user that the header of the request is reseved by the server and it will try response `

200’s =`the sucess code ,this is indicate that the request from the user was accepted`

300’s =`the location of  request from the user is not avaliable anymore `

400’s =`this indicate that there is problem in the client side  (client error code)`

500’s = `this indicate that there is problem in the server (Server error code)`

- What is a status code 202? `Accepted`

- What is a status code 308? ` Permanent Redirect`

- What code would you use if an update didn’t return data to a client?`204 `

- What code would you use if a resource used to exist but no longer does?`414 Request-URI Too Long`

- What is the ‘Forbidden’ status code?`403`

## Build A REST API With Node.js, Express, & MongoDB 

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

`to be able to connect it and use it `

2. What is middleware?

`basically is a function that will the receive the Request and Response objects`

3. What does app.use(express.json()) do?

`the middleware that used to recognize the incoming Request Object as a JSON Object.`

4. What does the /:id mean in a route?

`the id is a paramerter for this endpoint `

5. What is the difference between PUT and PATCH?

`PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource`

`PATCH method supplies a set of instructions to modify the resource`

6. How do you make a defalut value in a schema?

`inside the schema declaration we can put 'default' as property or method`

7. What does a 500 error status code mean?

` Internal Server Error server error response`

8. What is the difference between a status 200 and a status 201?
`200 OK => everything went good `

`201 Created =>  for create operations`