# Class 12 Reading Notes

## Status Codes REST methods

1. In your own words, describe what each group of status code represents:

100’s = Informational status code that lets the client know their request is being considered by the server.
200’s = Success code, the request was processed by the server.
300’s = Redirection code, the request is at a different location and a new request needs to be issued to the new location.
400’s = Invalid request code, issues a page not found or page inaccessible message.
500’s = Server error code, the client's request was correct but the server could not process.

2. What is a status code 202? In the create action via HTTP POST method, the request was recieved but not necessarily processed (in terms of asynchronous processing)

3. What is a status code 308? In the read action of the HTTP GET mthod, this is a permanent redirection to tell the client to use an entirely different URL to access the resource.

4. What code would you use if an update didn’t return data to a client? 204 No Content

5. What code would you use if a resource used to exist but no longer does? 410

6. What is the ‘Forbidden’ status code? 403, the client has no permissions to access the resource

## Build a REST API with Node.js, Express & MongoDB

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

- Want to use something that is not our local host.

2. What is middleware?

- app.use lets server accept json

3. What does app.use(express.json()) do? lets server accept json as a body instead of a post element or get element

4. What does the /:id mean in a route? /:id is used in the router.get function to get one object (in the case of the video it was to get one subscriber)

5. What is the difference between PUT and PATCH?

Patch updates based on user input for one piece of data, put updates all information beyond what the user inputs for entirety of data

6. How do you make a default value in a schema?

- use the keyword default

7. What does a 500 error status code mean?

- unexpected condition encountered by server so it cannot fulfill it's request

8. What is the difference between a status 200 and a status 201?

- 200 = everything is OK; 201 = created, server has fulfilled the request and created the resource

