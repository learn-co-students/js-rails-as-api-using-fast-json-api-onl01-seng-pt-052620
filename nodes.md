# Rails as an API
We can create a new rails app in API only mode using the `-api flag`

`rails new my_api --api`
This will skip middleware and files that are used to support a full stack web app in Rails. 
It will leave the pieces you need to build out a backend only API. 

What's sometimes confusing on the frontend is when you have

```js
fetch("/posts")
    .then(res => res.json())
```

We need to parse the body of the response as a JavaScript Data Structure before we work with it. 
We get a string in JSON(JavaScript Object Notation) format back from the API. 
We need to turn it into an object or an array before we work with it in our front end javascript. 