# Dnn.AuthServices.Jwt
More Secure version of DNN JWT Auth Service 

This repository is build on the [default DNN JWT Auth service](https://github.com/dnnsoftware/Dnn.Platform/tree/development/DNN%20Platform/Dnn.AuthServices.Jwt).
The only thing that is enhanced here is the way login credentials is passed to the `JwtAuth/API/mobile/login` endpoint.

Instead of passing the plain login credentials in the request body(used by DNN JWT Auth service), It will be more secure if we use the Basic Authentication technique
to pass the encoded login credentials in the request header(used in this Repo).

## How to use this
If you need to use this modified version of DNN JWT Auth service, First install the default DNN JWT Auth service by following
[these steps](http://www.dnnsoftware.com/docs/administrators/jwt/jwt-user-credentials.html) then replace the `Dnn.AuthServices.Jwt.dll` from `bin` with the dll file that you will get from the build of this repo.
