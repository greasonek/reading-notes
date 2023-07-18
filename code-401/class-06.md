# Class 06 Reading Notes

## Securing Passwords

1. Explain to a non-technical friend how you would safely hash and store a password.

- We use an algorithm that make cyber attacks slower and minimize the impact by using a technique called **key stretching**

2. What is Bcrypt?

- Bcrypt is an algorithm that uses key stretching to slow down brute-force search attacks hackers use to steal passwords.

3. Why might you use something like Bcrypt?

- Bcrypt is a function that can determine how slow a hash function will be meaning it can make an attack slower.

## Basic Auth

1. What is Basic Authentication?

- A method of HTTP user agent that provides a username and password when making a request.

2. What properties are necessary in the header of a Basic Auth request?

- username:password

3. How are username:password in Basic Auth encoded?

- A string that is encoded into an octet sequence.


## OWASP auth Cheatsheet

1. Define the authentication process to a non-technical recruiter.

- Authentication verifies an individual by the user submitting a username and password that only the user should know. Session Management is the process the server uses to maintain the entity interacting with it (like logging in with your gmail username/password)

2. How should your error messaging respond (both HTTP and HTML)? Why?

- In a generic manner such as 'user ID was incorrect' or 'account does not exist'
