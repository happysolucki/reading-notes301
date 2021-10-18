# Authentication

### OAuth

1\. What is OAuth?

OAuth is an open-standard authorization framework that describes how unrelated servers and services can safely allow authenticated access to their assets without sharing the initial, related, single logon credintial. OAuth tailors itself toward authorization.

2\. Give an example of what using OAuth would look like.

Whenever you login/signup on a website using third-party services like google, github, yahoo, etc.

3\. How does OAuth work? What are the steps that it takes to authenticate the user?

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

4\. What is OpenID?

OpenID is a framework that makes authentication easier.

### Authorization and Authentication flows

1\. What is the difference between authorization and authentication?

Authentication is the process of proving that you are who you say you are while authorization is the process of granting an authenticated user permission to do something.

2\. What is Authorization Code Flow?

An exchange of Authorization Code for a token.

3\. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

This is the Authorization Code Flow, but it introduces a secret called the Code Verifier. This adds security to the token exchange process. A malicious attacker can only intercept the Authorization Code, and they cannot exchange it for a token without the Code Verifier.

4\. What is Implicit Flow with Form Post?

This flow is only concerned with logging in. You would typically use this if you don't need access keys to invoke APIs. It removes the burden of obtaining and managing a secret.

5\. What is Client Credentials Flow?

Geared towards machine-to-machine applications, this flow authenticates and authorizes the app rather than a user.

6\. What is Device Authorization Flow?

A&A Flow that involves authentication on the device and in the browser.

7\. What is Resource Owner Password Flow?

A&A Flow which requests that users provide credentials (username and password), typically using an interactive form.
