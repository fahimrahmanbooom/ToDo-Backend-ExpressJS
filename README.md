
#TODO RestAPI Documentation

Developed By: Fahim Rahman
V1 Completion Date: 2 Aug 2021
V1 Last Update Date: 7 Aug 2021
Further Development: Yes
Technologies: NodeJS, ExpressJS, MongoDB, Cloudinary

---------------------------------------------------------
---------------------------------------------------------

!! SERVER SIDE USE ONLY !!

CHANGE PORT and IP: app.listen("Port", "Server IP")
INSTALL DEPENDENCIES: npm install
RUN SERVER: npm start

---------------------------------------------------------
---------------------------------------------------------

Live Server Base URL: https://todoexpressjs.herokuapp.com/

Restful APIs:
---------------------------------------------------------

Register:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/register
JSON BODY: { "email": string, "password": string, "confirmPassword": string }

---------------------------------------------------------

Login:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/login
JSON BODY: { "email": string, "password": string }

---------------------------------------------------------

Send OTP:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/sendOTP
JSON BODY: { "email": string }

---------------------------------------------------------

Forgot Password:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/forgotPassword
JSON BODY: { "email": string, "otp": string, "newPassword" : string, "newConfirmPassword": string }

---------------------------------------------------------

Refresh Token:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/refreshToken
JSON BODY: { "email": string, "refreshToken": string }

---------------------------------------------------------

Logout:

Request -> JSON BODY
API (POST): {baseURL}/api/v1/logout
JSON BODY: { "email": string, "refreshToken": string }

---------------------------------------------------------

TODO POST: 

Request -> Multi-Part FORM-DATA
API (POST): {baseURL}/api/v1/todo
BODY: image: file (optional), text: string
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

TODO GET All:

Response -> JSON BODY
API (GET): {baseURL}/api/v1/todo
HEADER: Authorization: Bearer {token} 

---------------------------------------------------------

TODO GET Single: 

Response -> JSON BODY
API (GET): {baseURL}/api/v1/todo/{todoID}
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

TODO PATCH Single: 

Request -> JSON BODY
API (PATCH): {baseURL}/api/v1/todo/{todoID}
JSON BODY: { "text": string, "isCompleted": bool }
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

DELETE Single: 

Request -> Nil
API (DELETE): {baseURL}/api/v1/todo/{todoID}
HEADER: Authorization: Bearer {token}

---------------------------------------------------------

DELETE All: 

Request -> Nil
API (DELETE): {baseURL}/api/v1/todo
HEADER: Authorization: Bearer {token} 

---------------------------------------------------------


---------------------------------------------------------
---------------------------------------------------------