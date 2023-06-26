# Intro to JWT:

# What is a JSON Web Token (JWT)?

*A JSON Web Token (JWT) is a compact and self-contained token format that is used for securely transmitting information between parties as a JSON object. It consists of three parts: a header, a payload, and a signature.*

### Header: The header of a JWT typically contains two parts: the type of token, which is JWT, and the signing algorithm being used, such as HMAC, RSA, or others. This header is Base64Url encoded.

### Payload: The payload of a JWT contains the claims, which are statements about an entity (typically the user) and additional metadata. Claims can include information like the user's identity, permissions, and other data relevant to the application. The payload is also Base64Url encoded.

### Signature: The signature is used to verify the integrity of the JWT and ensure that it hasn't been tampered with. It is created by taking the encoded header, encoded payload, a secret key (or a public/private key pair in case of asymmetric algorithms), and applying the signing algorithm specified in the header. The signature is appended to the encoded header and payload.

## When should we use JSON Web Tokens?

### JSON Web Tokens (JWTs) are commonly used when:
### Implementing stateless authentication: JWTs can securely authenticate and authorize users without the need for server-side sessions.
### Enabling cross-domain communication: JWTs can be easily transmitted and validated across different domains or services.
## Building microservices or APIs: JWTs provide a lightweight and secure way to authenticate and authorize requests between services.

## Claims are expected in which structural component of a JWT?

*Claims are expected to be included in the payload, which is the second structural component of a JSON Web Token (JWT).
The payload contains the statements or claims about an entity (such as a user) and additional metadata. These claims provide information about the entity's identity, permissions, and any other relevant data needed for the application's functionality.*

# Are JWTs Secure?
### JSON Web Tokens (JWTs) can be secure when implemented correctly:

*Use strong signing algorithms (e.g., HMAC, RSA) and keep signing keys secure to ensure token integrity.
Avoid storing sensitive information in the JWT payload; use encryption for confidentiality if needed.
Set appropriate token expiration times and enforce token validation to mitigate the risk of long-lived tokens.
Implement token revocation mechanisms to handle scenarios where tokens need to be invalidated before expiration.
Apply additional security measures such as rate limiting, secure token storage, and proper token transmission over HTTPS.* 

### If I get a JWT and I can decode the payload, how can we call that secure?
*While the ability to decode the payload of a JSON Web Token (JWT) may seem insecure, the security lies in the signature verification process that ensures the integrity of the token.
Decoding the payload alone does not grant access or tamper with the token's validity.
It is the signature validation that confirms the authenticity and prevents unauthorized modifications to the token.*

# JWTs Explained:
## Why use JWT?
JWTs (JSON Web Tokens) offer several advantages for authentication and authorization in applications:

*Stateless: JWTs are stateless, meaning servers don't need to store session information. This scalability simplifies server-side implementation.
Interoperability: JWTs are widely supported across different platforms and programming languages, making them highly versatile.
Security: JWTs can be digitally signed, ensuring data integrity and authentication. Additionally, they can be encrypted for confidentiality.
Lightweight: JWTs are compact in size, making them efficient for transmitting data over networks and reducing bandwidth usage.*

## JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

*Imagine you have a box that contains all the information you need for a specific task. This box is compact, meaning it doesn't take up much space.
It's also self-contained, meaning it holds everything you need without relying on anything external. This is similar to a JSON Web Token (JWT).
It's like a digital box that securely carries information from one place to another. This compact and self-contained nature makes it useful because you can easily send it over the internet without the need for extra resources or storing additional data.
It simplifies the process and ensures the information reaches its destination intact.*

## What are the three components (the structure) of a JWT signature?
*The structure of a JWT signature consists of three components: the encoded header, the encoded payload, and a secret key.
Firstly, the header contains information about the token type and the signing algorithm. Secondly, the payload holds the claims and additional data.
Both the header and payload are Base64Url encoded. Finally, the secret key, known only to the sender and the recipient, is used to create the signature.
The signature is generated by combining the encoded header and payload with the secret key using the specified signing algorithm*
. This three-component structure ensures the integrity and authenticity of the JWT.
