# Class 15 Reading Notes

## What is OAuth

1. What is OAuth?

- An authorization protocol framework that describes how unrelated servers and services can allow authenticated access to assets. A secure third party authorization. <a href="https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html">Source</a>

2. Give an example of what using OAuth would look like.

- Telling a social media platform that it's okay to for a third party to access your profile without giving that third party your password.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

- The first website connects to third party website on behalf of user and provides user's identity. The second site generates a one time token, the first site gives token to the user's client software which presents the token to their authorization provider. The client is asked to authenticate and then approve the authorization transaction to the second site. After approving, the user is given the access token to the first site which is then given to the second site as proof of authentification. The second site allows the first site to access their site on behalf of the user.

4. What is OpenID?

- OpenID is about authentification for humans to log into machines whereas OAuth is for machines to log into machines on behalf of humans. In 2014 is was reinvented as an authentification layer for OAuth

## Authorization and Authentification

1. What is the difference between authorization and authentication?

- Authenification verifies the identity of the user, authorization determines the user's access rights <a href="https://www.onelogin.com/learn/authentication-vs-authorization#:~:text=Authentication%20and%20authorization%20are%20two,authorization%20determines%20their%20access%20rights.">Source</a>

2. What is Authorization Code Flow?

- Exchanges the authentification code with a token, can be used for confidential apps and must be kept secure.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

- An extension to Authorization Code Flow that adds an extra bit of security because the token is sensitive info.

4. What is Implicit Flow with Form Post?

- Intended for apps that cannot securely stores client secrets. Requests tokns through front channgel without needing secrets or backend calls.

5. What is Client Credentials Flow?

- Authenticates and authorizes the app rather than the user.

6. What is Device Authorization Flow?

- Authorizes device the user is using to login, rather than authenticating the user directly.

7. What is Resource Owner Password Flow?

- Requests user provides credentials (username/password) using an interactive form, should only be used with Authorization Code Flow cannot be used
