# Class 15 Reading Assignment

## What is OAuth

1. OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

2. The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

3. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
The user approves (or their software silently approves) a particular transaction type at the first website.
The user is given an approved access token (notice it’s no longer a request token).
The user gives the approved access token to the first website.
The first website gives the access token to the second website as proof of authentication on behalf of the user.
The second website lets the first website access their site on behalf of the user.
The user sees a successfully completed transaction occurring.
OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

4. OpenID is an authentication protocol that allows users to authenticate with a website or application using an existing identity provider (IdP) rather than creating a new username and password for each site.

## Authorization and Authentication flows

1. Authentication is the process of verifying a user's identity, while authorization is the process of determining what actions or resources a user is authorized to access based on their identity.

2. Authorization Code Flow is an OAuth 2.0 flow used to obtain an access token from an authorization server by exchanging an authorization code. It is considered more secure than other OAuth flows because it requires a server-side secret to authenticate the client.

3. Authorization Code Flow with Proof Key for Code Exchange (PKCE) is an enhanced version of the Authorization Code Flow in OAuth 2.0 that provides an additional layer of security against authorization code interception attacks.

4. Implicit Flow with Form Post is an OAuth 2.0 flow used to obtain an access token for a user without using an authorization code. In this flow, the client (such as a web or mobile app) sends an authorization request to the authorization server, including its client ID and a redirect URI.

5. With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.

6. With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

7. Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.


## Things I want to know more about

### Resources

https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

https://auth0.com/docs/get-started/authentication-and-authorization-flow
