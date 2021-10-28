## Reading: Access Control (ACL)

### 1. When is Basic Authorization used vs. Bearer Authorization?

Basic authentication transmits credentials as user ID/password pairs, encoded using base64. Bearer authentication has security tokens called bearer tokens.

https://stackoverflow.com/questions/34013299/web-api-authentication-basic-vs-bearer

### 2. What does the JSON Web Token package do?

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

https://jwt.io/introduction

### 3. What considerations should we make when creating and storing a SECRET?

```plaintext
1. Never store unencryted secrets in git repos.
2. Store secrets safely.
3. Restrict API access and permissions.
4. Don't share secrets via messaging services.
```

https://res.cloudinary.com/da8kiytlc/image/upload/v1592031041/Cheatsheets/secrets_cheatsheet_bedizg.pdf

### Document the following Vocabulary Terms

#### 1. encryption

Encryption is the method by which information is converted into secret code that hides the information's true meaning.

https://searchsecurity.techtarget.com/definition/encryption

#### 2. token

An authentication token securely transmits information about user identities between applications and websites.

https://www.fortinet.com/resources/cyberglossary/authentication-token

#### 3. bearer

An HTTP authentication scheme that involves security tokens called bearer tokens.

https://swagger.io/docs/specification/authentication/bearer-authentication/

#### 4. secret

A Secret is an object that contains a small amount of sensitive data such as a password, a token, or a key.

https://kubernetes.io/docs/concepts/configuration/secret/

#### 5. JSON Web Token

JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

https://jwt.io/introduction
