## What is OAuth
1. What is OAuth?

`is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential `

2. Give an example of what using OAuth would look like.

` when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.`

3. How does OAuth work? What are the steps that it takes to authenticate the user?

* The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
* The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
* The first site gives this token and secret to the initiating user’s client software.
* The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
* If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
* The user approves (or their software silently approves) a particular transaction type at the first website.
* The user is given an approved access token (notice it’s no longer a request token).
* The user gives the approved access token to the first website.
* The first website gives the access token to the second website as proof of authentication on behalf of the user.
* The second website lets the first website access their site on behalf of the user.
* The user sees a successfully completed transaction occurring.
* OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. What is OpenID?

`is for humans logging into machines,`


## Authorization and Authentication flows

1. What is the difference between authorization and authentication?

|Authentication |  Authorization |
| ------------ | -------------|
| Determines whether users are who they claim to be  |Determines what users can and cannot access|
| Challenges the user to validate credentials (for example, through passwords, answers to security questions, or facial recognition)	  | Verifies whether access is allowed through policies and rules|
| Usually done before authorization	  | Usually done after successful authentication |
| Generally, transmits info through an ID Token	  | Generally, transmits info through an Access Token|
| Generally governed by the OpenID Connect (OIDC) protocol	  |Generally governed by the OAuth 2.0 framework|

2. What is Authorization Code Flow?

![authorization](https://images.ctfassets.net/cdy7uua7fh8z/2nbNztohyR7uMcZmnUt0VU/2c017d2a2a2cdd80f097554d33ff72dd/auth-sequence-auth-code.png)


3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

![Auth with proof](https://images.ctfassets.net/cdy7uua7fh8z/3pstjSYx3YNSiJQnwKZvm5/33c941faf2e0c434a9ab1f0f3a06e13a/auth-sequence-auth-code-pkce.png)

4. What is Implicit Flow with Form Post?

- The user clicks Login in the app.

- Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

- Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

- The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

- Your Auth0 Authorization Server redirects the user back to the app with an ID Token.

5. What is Client Credentials Flow?

* Your app authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (/oauth/token endpoint).

* Your Auth0 Authorization Server validates the Client ID and Client Secret.

* Your Auth0 Authorization Server responds with an Access Token.

* Your application can use the Access Token to call an API on behalf of itself.

* The API responds with requested data.


6. What is Device Authorization Flow?

![device](https://images.ctfassets.net/cdy7uua7fh8z/1A6jpG3W1H6SC9ZK92NyKd/40af53209f90a7c392f621f329fb4424/auth-sequence-device-auth.png)

7. What is Resource Owner Password Flow?

![password](https://images.ctfassets.net/cdy7uua7fh8z/4EeYNcnVX1RFcTy5z4lP4v/c3e4d22e6f8bf558caf07338a7388097/ROP_Grant.png)
