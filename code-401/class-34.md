# Class 34 Reading Notes

## Review API Server Build

1. Explain the difference between a query string parameter and a path parameter.

- Both are ways to pass info to a server in URLs, a **query string parameter** is an optional param that sends data to the server in key/value pairs following the '?' (if there are multiples they're separated by '&'). Example from the reading: <http://amazingapi.com/api/v1/products?category=electronics> *'?category=electronics' is the query string param*

- path params define the strucure of the URL and are essential. It is the param that directly appears in the URL path to access something specific like a product. Example from the reading: <http://amazingapi.com/api/v1/products/12345> *'12345' is the path param*

2. What would our API URL with a path id parameter be given the following information:
- Domain: <http://our-site.com>
- v3
- model name: stuff
- id: things

- <http://our-site.com/api/v3/stuff/things>

3. We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

- The interface is a user friendly way of dealing with a computer system without being an tech expert. The interface gives you a way to communicate to the API without understanding the inner workings, users can click buttons, enter information, choose options and this will send the user input info to the API server which will then respond to the user with what they ask for. It's similar to how drivers can drive a car and get where they need to go without being a mechanic, or a customer can go to a restaurant and order/recieve food without knowing how to cook it themselves.

## Review Auth Server Build

1. Describe how you would use middleware to implement basic and bearer auth.

- Basic auth uses middleware to signIn --> user sends a username and password and basic auth checks for credentials (does the username/password match what is stored in the database?), if all checks out, use next() to move forward with the request. The basic auth middleware will validate the user and return an object with a re-authentication/bearer token along with the user object.

- Bearer auth uses API tokens/JWTs (json web tokens) where the token would be tested against the database to see if it exists and uses next() if it does.

2. Describe the handshake necessary to implement OAuth.

- Oauth allows apps to get permission from users to access their data (like an app asking the user if they authorize it to access the photos from their Facebook page), the user must approve this access and the app will get a token to access the data. There are a few steps involved: the client (like Instagram) requests permission from the user to access their info from another resource (Facebook), the user approves by being redirected to Facebook to give approval, the client (Instagram) is provided with an auth code which it sends to Facebook, if the code is valid Facesbook will allow Instagram access to the users photos.

3. Describe how Role Based Access Control works to a non-technical friend.

- RBAC give certain people within a company more access to certain areas than others. For example, a regular employee would not have access to edit or delete a timesheet but a manager would. An employee would have access to their own office but a manager would have access to all rooms in a building. RBAC gives everyone the access they need to do their job.
