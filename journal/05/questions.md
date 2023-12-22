# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > Create, read, update, delete

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > To create you use post, to read you use get, to update you use put, & delete is delete

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > ORM stands for object relational mapping. Mongoose is the ORM that we use. 

04. Which two `HTTP` request types include a body?

  > push & post

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > synchronous, asynchronous

06. What are the three types of data relationships? Provide an example of each.

  > One to one, one to many, and many to many. 
  Colonies on planets are a one to one because one colony is on one planet. Planets to galaxies is a one to many, because each planet could only be connected to one galaxy but that galaxy could be connected to many planets. The species interacting with the planets was a many to many because many species could be on any planet, & every species could be on many different planets.
  
07. What is middleware?

  > middleware is software that communicates between the database and the application. We are also using middleware when we authenticate users & do a check for their barer token to access parts of our site.

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks. 

  > request, response

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > GET /seasons?tag=winter

10. What is a ***virtual property***?

  > A virtual property is a javascript function that creates properties based on values in an element. Mongoose defines virtual properties with GET and SET
