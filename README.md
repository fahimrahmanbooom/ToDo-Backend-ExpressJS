<p><br></p>
<p>#TODO RestAPI Documentation</p>
<p><br></p>
<p>Developed By: Fahim Rahman</p>
<p>V1 Completion Date: 2 Aug 2021</p>
<p>V1 Last Update Date: 7 Aug 2021</p>
<p>Further Development: Yes</p>
<p>Technologies: NodeJS, ExpressJS, MongoDB, Cloudinary</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>!! SERVER SIDE USE ONLY !!</p>
<p><br></p>
<p>CHANGE PORT and IP: app.listen(&quot;Port&quot;, &quot;Server IP&quot;)</p>
<p>INSTALL DEPENDENCIES: npm install</p>
<p>RUN SERVER: npm start</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Live Server Base URL: https://todoexpressjs.herokuapp.com/</p>
<p><br></p>
<p>Restful APIs:</p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Register:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/register</p>
<p>JSON BODY: { &quot;email&quot;: string, &quot;password&quot;: string, &quot;confirmPassword&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Login:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/login</p>
<p>JSON BODY: { &quot;email&quot;: string, &quot;password&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Send OTP:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/sendOTP</p>
<p>JSON BODY: { &quot;email&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Forgot Password:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/forgotPassword</p>
<p>JSON BODY: { &quot;email&quot;: string, &quot;otp&quot;: string, &quot;newPassword&quot; : string, &quot;newConfirmPassword&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Refresh Token:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/refreshToken</p>
<p>JSON BODY: { &quot;email&quot;: string, &quot;refreshToken&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>Logout:</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (POST): {baseURL}/api/v1/logout</p>
<p>JSON BODY: { &quot;email&quot;: string, &quot;refreshToken&quot;: string }</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>TODO POST:&nbsp;</p>
<p><br></p>
<p>Request -&gt; Multi-Part FORM-DATA</p>
<p>API (POST): {baseURL}/api/v1/todo</p>
<p>BODY: image: file (optional), text: string</p>
<p>HEADER: Authorization: Bearer {token}</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>TODO GET All:</p>
<p><br></p>
<p>Response -&gt; JSON BODY</p>
<p>API (GET): {baseURL}/api/v1/todo</p>
<p>HEADER: Authorization: Bearer {token}&nbsp;</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>TODO GET Single:&nbsp;</p>
<p><br></p>
<p>Response -&gt; JSON BODY</p>
<p>API (GET): {baseURL}/api/v1/todo/{todoID}</p>
<p>HEADER: Authorization: Bearer {token}</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>TODO PATCH Single:&nbsp;</p>
<p><br></p>
<p>Request -&gt; JSON BODY</p>
<p>API (PATCH): {baseURL}/api/v1/todo/{todoID}</p>
<p>JSON BODY: { &quot;text&quot;: string, &quot;isCompleted&quot;: bool }</p>
<p>HEADER: Authorization: Bearer {token}</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>DELETE Single:&nbsp;</p>
<p><br></p>
<p>Request -&gt; Nil</p>
<p>API (DELETE): {baseURL}/api/v1/todo/{todoID}</p>
<p>HEADER: Authorization: Bearer {token}</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p>DELETE All:&nbsp;</p>
<p><br></p>
<p>Request -&gt; Nil</p>
<p>API (DELETE): {baseURL}/api/v1/todo</p>
<p>HEADER: Authorization: Bearer {token}&nbsp;</p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p><br></p>
<p><br></p>
<p>---------------------------------------------------------</p>
<p>---------------------------------------------------------</p>
