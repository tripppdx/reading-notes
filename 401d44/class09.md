## Reading: Authorization/Authentication

### 1. What header(s) are used in authentication and authorization

The authentication header is basic with base64 username and password. The authorization header is bearer with a token

### 2. What is safe to put into a JWT

The JWT is safe to contain a token and a secret.

### 3. How are JWTs validated

```javascript
jwt.verify();
```

### Define:

#### 1. RBAC

RBAC stands for Role-Based Access Control.

#### 2. User Roles

User roles define the level of access a particular user is granted based on an ACL (acces control list) paradigm. These roles determine what CRUD a user can do.

#### 3. JWT Token

JSON Web Token
