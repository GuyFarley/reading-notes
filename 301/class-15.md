# Code 301 - Class 15 - Authentication

## [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

1. What is OAuth? OAuth is an authorization protocol that describes how servers can allow authenticated access to their assets without sharing the initial logon credentials.

2. Give an example of what using OAuth would look like. When you go to log in to a website and it offers to log you in using another service's login (like google or microsoft).

3. How does OAuth work? What are the steps that it takes to authenticate the user? According to [this article](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html):

> - The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
> - The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
> - The first site gives this token and secret to the initiating user’s client software.
> - The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
> - If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
> - The user approves (or their software silently approves) a particular transaction type at the first website.
> - The user is given an approved access token (notice it’s no longer a request token).
> - The user gives the approved access token to the first website.
> - The first website gives the access token to the second website as proof of authentication on behalf of the user.
> - The second website lets the first website access their site on behalf of the user.
> - The user sees a successfully completed transaction occurring.

4. What is OpenID? While it started as a single sign-in tool, it has since shifted to become an authentication layer for OAuth.
>
> - OAuth = authorization
> - OpenID = authentication

## [Authorization and Authentication flows](https://auth0.com/docs/get-started/authentication-and-authorization-flow)

1. What is the difference between authorization and authentication?

2. What is Authorization Code Flow? It exchanges an Authorization Code for a token.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)? This process uses a "secret" that is created by the calling application, which can then be verified by the authorization server

4. What is Implicit Flow with Form Post? It is designed for application that are unable to store Client Secrets. It is not best practice, but is a more streamlined workflow for apps that only need an ID token for user authentication

5. What is Client Credentials Flow? This is for M2M (machine-to-machine) apps. It differs from Authorization Code Flow in that it allows the app to pass along a Client ID and Secret to authenticate itself and get a token.

6. What is Device Authorization Flow? With this flow, an input-constrained device asks a user to go to a link on their computer, smartphone, etc. and authorize the device. (I'm sure I've done this several times with my Roku device).

7. What is Resource Owner Password Flow? Simply requesting a username and password through an interactive form (not ideal because of lower security).

[Back to Home](../README.md)
