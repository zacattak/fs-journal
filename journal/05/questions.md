# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  >CRUD stands for Create, Read, Update and Delete.

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > The HTTP methods for create are 'POST' and 'PUT', the method for read is 'GET', the method for update is 'PUT' and 'PATCH', the method for delete is 'DELETE'.

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > 'ORM' stands for object relational mapping. Mongoose is the 'ORM' we use when interacting with MongoDB.

04. Which two `HTTP` request types include a body?

  > 'POST' and 'PUT' HTTP request types include a body.

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > synchronous, asynchronous

06. What are the three types of data relationships? Provide an example of each.

  > One to One, One to many, and many to many. A good example of a one-to-one relationship could be the relationship between a 'user' and their singular 'password'. An example of a one to many relationship could be the relationship between a given 'class' and its 'students'. An example of a many to many relationship could be the relationship between (many) 'books' and (many) 'authors'.

07. What is middleware?

  > Middleware can be thought of as a form of software that connects applications and operating systems.

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > request, response

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  >const res = await axios.get('http://localhost:3000/test?tag=winter')
  Not sure if I understood the question correctly, I referred to the reading section about query parameters and appending to the url.

10. What is a ***virtual property***?

  > A virtual property refers to a property that exists ONLY in online spaces.
