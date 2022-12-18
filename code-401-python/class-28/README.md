# Reading 33: Authentication and Production Server

## [JSON Web Tokens](https://jwt.io/introduction/)

* JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

  * Authorization: This is the most common scenario for using JWT.

  * Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties.

### Payload

* Payload The second part of the token is the payload, which contains the claims.
* Claims are statements about an entity (typically, the user) and additional data.
* There are three types of claims: registered, public, and private claims.

* **Registered claims**: These are a set of predefined claims which are not mandatory but recommended, to provide a set of useful, interoperable claims. Some of them are: iss (issuer), exp (expiration time), sub (subject), aud (audience), and others.

* **public claims**: These can be defined at will by those using JWTs. But to avoid collisions they should be defined in the IANA JSON Web Token Registry or be defined as a URI that contains a collision resistant namespace.
* **Private claims**: These are the custom claims created to share information between parties that agree on using them and are neither registered or public claims.

## [DRF JWT Authentication](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

* token should be included in all requests
* installation and set up
  * pip install djangorestframework_simplejwt
  * settings.py
    * REST_FRAMEWORK authentication
  * urls.py
    * token path and token refresh path
  * obtain token
  * token lasts five minutes
  * to get a new token refresh the token refresh endpoint
* refresh token allows for speed by removing uneeded steps
* refresh toekn allows for better security

## [Django Runserver Is Not Your Production Server](https://build.vsupalov.com/django-runserver-in-production/)

* using a WSGI server and more specifically a Gunicorn server for deployment; server: Nginx
* runserver command is not meant for production
* function is called when the request comes in and passes that info to function and then responds with corrently formated data

## Bookmark

* [JWT with DRF](https://www.youtube.com/watch?v=Fhcn2qx-4VQ)
* [Gunicorn](https://gunicorn.org/)
* [Django Migrations Primer](https://realpython.com/django-migrations-a-primer/)
