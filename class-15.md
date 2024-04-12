# table of contents
## code 301 reading notes
## Class 15 reading notes
### Reading Class 15, 12 APR

# Reading 1: [https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html](#)

### 1. What is OAuth?
OAuth (Open Authorization) is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites but without giving them the passwords. This is done through tokens instead of credentials, which allows the data sharing service to authorize specific account information to be shared without exposing the user's full account credentials.

### 2. Example of Using OAuth:
Imagine you want to log into Zoom but don't want to create a new account. Instead, you choose to log in using your existing Google account. When you select "Login with Google," the music service redirects you to a Google login page. After you authenticate with Google, it asks if you are willing to let Zoom access parts of your Google account (like your email address). Once you agree, Google sends a token to Zoom, which can use it to access the agreed-upon information without ever seeing your password.

### 3. How OAuth Works:
Here are the typical steps involved in OAuth authentication:
- **User Authorization:** The user initiates the process on the client application (like clicking "Log in with Google") and is redirected to the service that owns the account (the authorization server).
- **Authentication:** The user logs into the authorization server and grants the client application permission to access their information.
- **Token Exchange:** Upon successful authentication and authorization, the authorization server issues an access token to the client application.
- **Access Granted:** The client application uses this access token to access the user's information from the resource server under the permissions that were granted.

### 4. What is OpenID?
OpenID is a decentralized authentication protocol that allows users to be authenticated by certain co-operating sites (known as Relying Parties, RP) using a third-party service. It extends OAuth by allowing authentication as well as authorization, meaning it can convey not just that a user has authorized an application, but also information about who the user is. This "identity layer" built on top of OAuth allows users to sign into different sites with the same digital identity, which can help reduce password fatigue and the need for multiple usernames and passwords.

# Reading 2: [https://auth0.com/docs/flows](#)

### 1. Difference Between Authorization and Authentication:
- **Authentication:** is the process of verifying who a user is, typically by checking if their credentials match those in a database of authorized users. It answers the question, "Are you who you say you are?"
- **Authorization:** occurs after the system knows the user's identity and involves determining the access level or permissions that the user should have. It answers the question, "Are you allowed to access this resource?"

### 2. Authorization Code Flow:
The Authorization Code Flow is an OAuth 2.0 flow specifically designed for client-server communication where the client can securely maintain a client secret. The flow goes as follows:
1. The application redirects the user to an authorization server with a request for authorization.
2. The user authenticates and authorizes the application.
3. The authorization server sends a short-lived authorization code to the application.
4. The application exchanges the authorization code for an access token, often using a client secret for additional security.
5. The access token can then be used to make API calls to access protected resources on behalf of the user.

### 3. Authorization Code Flow with Proof Key for Code Exchange (PKCE):
PKCE is an enhancement to the Authorization Code Flow that prevents certain attacks, such as the authorization code interception attack, and is particularly useful for public or native clients where the client secret cannot be securely stored. In PKCE:
- The client generates a secret called a Code Verifier and its transformation, called the Code Challenge.
- When initiating the flow, the client sends the Code Challenge to the authorization server.
- After the user authorizes, the client receives an authorization code and must send the Code Verifier to the authorization server along with the authorization code for verification.
- If the verification succeeds, the client is granted an access token.

### 4. Implicit Flow with Form Post:
The Implicit Flow with Form Post is a simplified OAuth flow that was historically recommended for clients without a client secret, such as JavaScript-based browser apps. This flow returns tokens directly in an HTTP form post response instead of through a redirect URI. It is less secure than other flows and generally not recommended, especially with the advancement of more secure methods like PKCE.

### 5. Client Credentials Flow:
This OAuth flow is used for server-to-server communication where the application acts on its own behalf rather than on behalf of a user. The application requests an access token using only its client credentials (client ID and secret) and, if authenticated, the authorization server grants the access token. This token is then used for the API calls that do not involve user data.

### 6. Device Authorization Flow:
This flow is used for devices that either do not have a browser or have input constraints (like smart TVs, IoT devices). It works as follows:
1. The device displays a URL and a code to the user.
2. The user visits the URL on a secondary device (like a smartphone) and inputs the code.
3. The user authorizes the device after logging in, if necessary.
4. The device polls the authorization server and eventually receives an access token to access the user's data.

### 7. Resource Owner Password Flow:
This OAuth flow involves a user providing their service credentials (username and password) directly to the application, which then uses them to obtain an access token from the authorization server. This flow is considered less secure as it exposes the user's credentials to the application and should only be used when other flows are not viable, typically in legacy systems or highly trusted applications.


# Things I want to know more about.
### https://auth0.com/docs/libraries/auth0-react