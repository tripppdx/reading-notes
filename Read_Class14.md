# Readings: Authentication

## What is OAuth

### 1. What is OAuth?

OAuth is a protocol/framwework that allows authenticated access to unrelated resources using a single logon credential without actually sharing it.

### 2. Give an example of what using OAuth would look like.

When yot got to Netlify and can sign in via Gihub who does the authentication without sharing your password with Netlify.

### 3. How does OAuth work? What are the steps that it takes to authenticate the user?

```
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.
```

### 4. What is OpenID?

OpenID is a service that that was originally conceived to provide user authentication across all websites that implemented it. Today it is an authentication layer fro OAuth.

## Authorization and Authentication flows

### 1. What is the difference between authorization and authentication?

Authentication is the process of verifying the identity of a user while authorization is the process of identifying what that user has access to.

### 2. What is Authorization Code Flow?

This is the exchange of an authorization code for a token

### 3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

```
1. The user clicks Login within the regular web application.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint).

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.

5. Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.

6. Auth0's SDK sends this code to the Auth0 Authorization Server (/oauth/token endpoint) along with the application's Client ID and Client Secret.

7. Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.

8. Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

9. Your application can use the Access Token to call an API to access information about the user.

10. The API responds with requested data.

https://auth0.com/docs/authorization/flows/authorization-code-flow
```

### 4. What is Implicit Flow with Form Post?

```
1. The user clicks Login in the app.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

5. Your Auth0 Authorization Server redirects the user back to the app with an ID Token.

https://auth0.com/docs/authorization/flows/implicit-flow-with-form-post
```

### 5. What is Client Credentials Flow?

```
1. Your app authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (/oauth/token endpoint).

2. Your Auth0 Authorization Server validates the Client ID and Client Secret.

3. Your Auth0 Authorization Server responds with an Access Token.

4. Your application can use the Access Token to call an API on behalf of itself.

5. The API responds with requested data.

https://auth0.com/docs/authorization/flows/client-credentials-flow
```

### 6. What is Device Authorization Flow?

Device authorization flow allows a user to authenticate via a link rather that enterign a password.

### 7. What is Resource Owner Password Flow?

```
1. The user clicks Login within the application and enters their credentials.

2. Your application forwards the user's credentials to your Auth0 Authorization Server (/oauth/token endpoint).

3. Your Auth0 Authorization Server validates the credentials.

4. Your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token).

5. Your application can use the Access Token to call an API to access information about the user.

6. The API responds with requested data

https://auth0.com/docs/authorization/flows/resource-owner-password-flow
```
