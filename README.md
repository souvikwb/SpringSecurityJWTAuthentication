# SpringSecurityJWTAuthentication
This is a simple example of spring jwt authentication. In pom.xml we have added this 2 dependency, 1. jjwt, 2. jaxb-api. 
We have used "/authenticate" end point to generate jwt token, and for other end points we have to pass this jwt token as a header, then only it can authenticate the request.
We extended "OncePerRequestFilter" and overrided "doFilterInternal" method to validate the jwt token for each incoming request.
