## Reading: Bearer Authorization

### 1. Write the following steps in the correct order:

```plaintext
1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Redirect to a third party authentication endpoint
4. Receive authorization code
5. Make a request to the access token endpoint
6. Receive access token
7. Make a request to a third-party API endpoint
```

### 2. What can you do with an authorization code?

You can use an authorization code to request an access token

### 3. What can you do with an access token?

You can use the token to access a secure API.

### 4. What’s a benefit of using OAuth instead of your own basic authentication?

### Document the following Vocabulary Terms

#### 1. Client ID

The client_id is a public identifier for apps

https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/

#### 2. Client Secret

The client_secret is a secret known only to the application and the authorization server.

https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/

#### 3. Authentication Endpoint

The authentication endpoint is used confirm the identity of the client requesting a resource. It provides an authorization code which can be redeemed for a token from the access token enpoint.

https://auth0.com/docs/authorization/flows/authorization-code-flow

#### 4. Access Token Endpoint

The token access endpoint exchanges the authorization code, client id and client secret for a token.

https://www.ibm.com/docs/en/sva/9.0.7?topic=endpoints-token-endpoint
https://www.oauth.com/oauth2-servers/client-registration/client-id-secret/

#### 5. API Endpoint

The protected resource that requires a token for access.

#### 6. Authorization Code

Code issued by the authorization endpoint which can be redeemed for a token.

#### 7. Access Token

A code that can contain user info , permissions, groups, and timeframes that allows access to secure resources.

https://www.okta.com/identity-101/access-token/
