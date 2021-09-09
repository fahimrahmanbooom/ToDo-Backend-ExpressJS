##TODO RestAPI Documentation

Developed By: Fahim Rahman<br>
V1 Completion Date: 2 Aug 2021<br>
V1 Last Update Date: 7 Aug 2021<br>
Further Development: Yes<br>
Technologies: NodeJS, ExpressJS, MongoDB, Cloudinary

---------------------------------------------------------
---------------------------------------------------------

!! SERVER SIDE USE ONLY !!

CHANGE PORT and IP: app.listen("Port", "Server IP")<br>
INSTALL DEPENDENCIES: npm install<br>
RUN SERVER: npm start

---------------------------------------------------------
---------------------------------------------------------

Live Server Base URL: https://todoexpressjs.herokuapp.com/

Restful APIs:
---------------------------------------------------------

Register:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/register<br>
JSON BODY: { "email": string, "password": string, "confirmPassword": string }

---------------------------------------------------------

Login:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/login<br>
JSON BODY: { "email": string, "password": string }

---------------------------------------------------------

Send OTP:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/sendOTP<br>
JSON BODY: { "email": string }

---------------------------------------------------------

Forgot Password:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/forgotPassword<br>
JSON BODY: { "email": string, "otp": string, "newPassword" : string, "newConfirmPassword": string }

---------------------------------------------------------

Refresh Token:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/refreshToken<br>
JSON BODY: { "email": string, "refreshToken": string }

---------------------------------------------------------

Logout:

Request -> JSON BODY<br>
API (POST): {baseURL}/api/v1/logout<br>
JSON BODY: { "email": string, "refreshToken": string }

---------------------------------------------------------

TODO POST: 

Request -> Multi-Part FORM-DATA<br>
API (POST): {baseURL}/api/v1/todo<br>
BODY: image: file (optional), text: string<br>
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

TODO GET All:

Response -> JSON BODY<br>
API (GET): {baseURL}/api/v1/todo<br>
HEADER: Authorization: Bearer {token} 

---------------------------------------------------------

TODO GET Single: 

Response -> JSON BODY<br>
API (GET): {baseURL}/api/v1/todo/{todoID}<br>
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

TODO PATCH Single: 

Request -> JSON BODY<br>
API (PATCH): {baseURL}/api/v1/todo/{todoID}<br>
JSON BODY: { "text": string, "isCompleted": bool }<br>
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

DELETE Single: 

Request -> Nil<br>
API (DELETE): {baseURL}/api/v1/todo/{todoID}<br>
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

DELETE All: 

Request -> Nil<br>
API (DELETE): {baseURL}/api/v1/todo<br>
HEADER: Authorization: Bearer {token} 

---------------------------------------------------------


---------------------------------------------------------
---------------------------------------------------------
