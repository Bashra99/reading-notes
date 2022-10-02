# Reading 15: Authentication

## [Reading: What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

### What is OAuth?

"OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential."

### Give an example of what using OAuth would look like

When you log onto a site and it allow you to sign in using a thrid party like Google or Facebook, that is Oauth.

### How does OAuth work? What are the steps that it takes to authenticate the user?

Oauth takes the information given to it, authenticates that it is indeed the user with a token assigned and then gives the running code a response saying that it was or was not authenticated.

### What is OpenID?

OpenID authenticates users and allows for a single sign in.

## [Reading: Authorization and Authentication flows](https://auth0.com/docs/flows)

### What is the difference between authorization and authentication?

Authentication is verifying that you are who you say you are when logging into something. Authorization determines how you have access to ceratin resources.

### What is Authorization Code Flow?

Authorization Code Flow is the flow of the token the user is given. This must use server code so that it not available to the user to see.

### What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

It is very similar to authorization code flow but there is a differnet step that uses a proof key.

### What is Implicit Flow with Form Post?

This is an alternative to authorization code flow for apps that cannot securely store there user information. This is no longer best practice, but still can and is used.

### What is Client Credentials Flow?

This flow checks for authorization and authentication of the app instead of the user.

### What is Device Authorization Flow?

This flow allows the user to click a link on there device and the device itself is authenticated instead of the user.

### What is Resource Owner Password Flow?

This is a flow that is not recommended and should only be used when other methods are not an option.

### Things I want to know more about
- SQL

