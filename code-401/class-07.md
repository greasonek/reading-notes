# Class 07 Reading Notes

## Intro to JWT

1. What is a JSON Web Token (JWT)?

- JSON web token - way for securely transmitting info between parties as a JSON object

2. When should we use JSON Web Tokens?

- Authorization, info exchange

3. Claims are expected in which structural component of a JWT?

- payload

## Are JWTs secure?

1. If I get a JWT and I can decode the payload, how can we call that secure?

- JWTs can be signed but not encrypted, if you don't know the private key you can't change it

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

- the key

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

- by use of the hash function Hsh(payload + secret) we can check if the signatures match

## JWTs Explained

1. Why use JWT?

2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

3. What are the three components (the structure) of a JWT signature?
