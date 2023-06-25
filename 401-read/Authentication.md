# Securing Passwords
## Explain to a non-technical friend how you would safely hash and store a password: 
### To safely hash and store a password:
*Use a secure hashing algorithm like bcrypt or Argon2.
Generate a unique salt for each password and append it before hashing.
Store the hashed password and the corresponding salt securely in a database.
By following these steps, the password is protected by a one-way hash function, making it computationally infeasible to reverse engineer the original password even if the stored information is compromised.*

## What is Bcrypt?
*Bcrypt is a widely-used cryptographic algorithm for password hashing.
It is designed to be slow and computationally expensive, making it resistant to brute-force and dictionary attacks.
Bcrypt incorporates a salt value and multiple rounds of hashing, enhancing the security of the hashed passwords.*

 ## Why might you use something like Bcrypt?
 *Bcrypt provides a high level of security by incorporating a salt and multiple rounds of hashing, making it difficult for attackers to crack passwords.
It helps protect user passwords in case of a data breach, as the original passwords are not stored and cannot be easily reversed from the hashed values.
Bcrypt's computational cost slows down brute-force and dictionary attacks, adding an additional layer of defense against unauthorized access.*

# Basic Auth:
## What is Basic Authentication?
*Basic Authentication is a simple method for user authentication over HTTP.
It involves sending a username and password in plain text as part of the request headers.
Basic Authentication is considered relatively insecure, and it is recom
mended to use it over secure connections (HTTPS) or employ more advanced authentication mechanisms.*

## What properties are necessary in the header of a Basic Auth request?
*The Authorization header field to indicate the use of Basic Authentication.
The value of the Authorization field should be in the format: Basic <base64-encoded-credentials>.
The base64-encoded credentials consist of the username and password concatenated with a colon (username:password), encoded using base64 encoding.*

## How are username:password in Basic Auth encoded?
*Concatenate the username and password with a colon: username:password.
Convert the resulting string (username:password) to bytes using a specific character encoding (e.g., UTF-8).
Encode the bytes using base64 encoding.
Prepend the encoded string with the word "Basic" followed by a space: Basic <base64-encoded-credentials>.
Include this value in the Authorization header of the HTTP request.*

# OWASP auth cheatsheet:
## Define the authentication process to a non-technical recruiter.
*Authentication is the process of verifying the identity of a user.
It typically involves providing credentials (e.g., username and password) to prove ownership of an account.
Authentication ensures that only authorized individuals can access protected resources or perform specific actions within a system.*

## How should your error messaging respond (both HTTP and HTML)? Why?
*Error messaging should provide clear and informative responses:
HTTP responses should include appropriate status codes (e.g., 400 for bad request, 404 for not found) to indicate the nature of the error.
HTML error pages should provide user-friendly messages explaining the error and potential solutions, helping users understand and resolve the issue.
Clear and consistent error messaging improves user experience, facilitates troubleshooting, and enhances overall system usability.*
 ### Looking ahead at this module’s course schedule, What do you look forward to learning?
 * knowing more about security and how to make the password more stronger and how to fetch it with frontEnd 
