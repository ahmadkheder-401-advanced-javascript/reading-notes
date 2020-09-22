# JsonWebToken
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
__Here are some scenarios where JSON Web Tokens are useful:__
* **Authorization**: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. 
* **Information Exchange**: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. 

### JSON Web Token structure Consist of :

    Header
    Payload
    Signature
## IS JWT secure?
JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.


# Term

- **ClientID**: The client_id is a public identifier for apps
- **Client Secret**:A client secret is a secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors. Protect your client secrets and never include them in mobile or browser-based apps.
- **Authentication Endpoint**:  is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service. ... Authenticating both the user and the device can provide two-factor authentication
- The **authorization code**: is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.
- An **access token**: is an opaque string that identifies a user, app, or Page and can be used by the app to make graph API calls. When someone connects with an app using Facebook Login and approves the request for permissions, the app obtains an access token that provides temporary, secure access to Facebook APIs.
