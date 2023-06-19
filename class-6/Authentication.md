# Authentication

## 1- Securing Passwords

### Explain to a non-technical friend how you would safely hash and store a password?

Using a lockbox analogy, we can think of password hashing as putting a password inside a lockbox and securing it. The lockbox represents a secure algorithm that transforms the password into a unique and irreversible code. The locked password is then stored in a secure place, such as a database. When you want to verify the password, you compare the newly locked password with the stored locked password. This way, even if someone gains access to the stored passwords, they won't be able to retrieve the original passwords.

### What is Bcrypt?

Bcrypt is a secure and widely-used password hashing algorithm. It takes a plain-text password and transforms it into a hashed version that is extremely difficult to reverse or decode. Bcrypt incorporates built-in salting and multiple rounds of encryption, making it resistant to various password cracking techniques. This ensures that even if a hacker gets access to the hashed passwords, it would be highly challenging to retrieve the original password.

### Why might you use something like Bcrypt?

Bcrypt provides strong security for storing passwords by making them extremely difficult to crack

## 2- Basic Auth

### What is Basic Authentication?

Basic Authentication is a simple and widely used authentication method for web applications. It involves sending the username and password credentials in plain text over the network. The server verifies the credentials and grants access if they are valid. However, Basic Authentication is considered less secure than other methods because the credentials are not encrypted during transmission, making them vulnerable to interception.

### What properties are necessary in the header of a Basic Auth request?

The value for Basic Authentication is typically in the format "Basic base64(username:password)".

```
Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

```

### How are username:password in Basic Auth encoded?

Concatenate the username and password with a colon: "myusername:mypassword".
Encode the resulting string using Base64 encoding, resulting in: "bXl1c2VybmFtZTpteXBhc3N3b3Jk".

### Define the authentication process to a non-technical recruiter.

authentication involves confirming the identity of a user by verifying their provided credentials against the stored credentials. This process ensures that only authorized individuals can access protected resources or perform specific actions within a system.

### How should your error messaging respond (both HTTP and HTML)? Why?

Error messaging in HTTP (status codes) and HTML should be clear and informative:

HTTP status codes communicate the outcome of a request (e.g., 404 for Not Found, 500 for Internal Server Error).
HTML error pages provide user-friendly explanations and guidance to resolve errors.
Effective error messaging improves user experience, troubleshooting, and builds trust in the application or website.

### How are username:password in Basic Auth encoded?

Concatenate the username and password with a colon: "myusername:mypassword".
Encode the resulting string using Base64 encoding, resulting in: "bXl1c2VybmFtZTpteXBhc3N3b3Jk".
