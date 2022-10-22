# refresh-token-jwt-nodejs-authentication



Nodejs Authentication Using JWT and Refresh Token

Nodejs authentication using JWT a.k.a JSON web token is very useful when you are developing a cross-device authentication mechanism.

Here is how token-based authentication works:

User logins to the system and upon successful authentication, the user are assigned a token which is unique and bounded by time limit say 15 minutes On every subsequent API call, the user provides the access token in order to consume the system resources. When time is expired, the user has to login again to get a new token The last step is frustrating, we can’t ask users to log in each and every single time once the token is expired.

There are two ways to solve this:

Increase the time of the token Use refresh token to extend the token I have covered token-based authentication in this article in detail.

In this Nodejs authentication tutorial, I am going to build a simple/boilerplate solution to handle the refresh token mechanism in Nodejs authentication.

Testing the code Let’s do some testing.

Run the code using the following command.

node server.js Open your favorite API testing tool, mine is Postman, and hit the /login API route.

URL: http://localhost:3000/api/login body: { "email": "suraj@kodingnotes.com", "name": "Suraj" }
