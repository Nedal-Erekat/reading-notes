
## What is JSON Web Token?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

JWT is a very modern, simple and secure approach which extends for Json Web Tokens. Json Web Tokens are a stateless solution for authentication.

Assuming we already have a registered user in our database. So the user's client starts by making a post request with the username and the password, the application then checks if the user exists and if the password is correct, then the application will generate a unique Json Web Token for only that user.

## JWT, how are they secure?
JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.

## When should you use JSON Web Tokens?
1. Authorization
2. Information Exchange

## What is the JSON Web Token structure?

* Header
* Payload
* Signature