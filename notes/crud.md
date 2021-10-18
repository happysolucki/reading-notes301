# CRUD

1\. Describe what eaxch group of status code represents:

- 100's = Informational
- 200's = Success
- 300's = Redirection
- 400's = Client Error
- 500's = Server Error

2\. What is status code 202?

Signals to the client that the request has been accepted, but its processing will finish some time in the future. This status code is typically used for asynchronous requests.

3\. What is status code 308?

This code is for permanent redirects. It tells the client to use another URL to access the resource and not use the current URL anymore.

4\. What code would you use if an update didn't return data to a client?

204

5\. What code would you use if a resource used to exist but no longer does?

410

6\. What is the 'Forbidden' status code?

403

### Node.js, Express, and MongoDB

1\. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

For general security and to make it easier to specify where your database is hosted

2\. What is middleware?

Code that runs when the server gets a request but before it gets passed to any routes

3\. What does `app.use(express.json())` do?

It allows your backend server to accept json

4\. What does the `/:id` mean in a route?

It signifies a parameter being passed to this route. In this case, the parameter can be accessed by `req.params.id`.

5\. What is the difference between `PUT` and `PATCH` ?

`PATCH` partially updates data while `PUT` wholly updates it

6\. How do you make a default value in a schema?

`default: what you want it to default to`

Ex.

```js
name: {
  type: String,
  default: 'Joe'
}
```

7\. What does a `500` error status code mean?

It means that there's a server-side error

8\. What is the difference between a status `200` and a status `201` ?

`200` is a general success code while `201` is a more specific one which signals that something was created

#### References

[Stats Codes Based on REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[Build A REST API With Node.js, Express, & MongoDB](https://www.youtube.com/watch?v=fgTGADljAeg)
