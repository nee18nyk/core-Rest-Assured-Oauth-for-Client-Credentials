# core-Rest-Assured-Oauth-for-Client-Credentials
- Automated for Client credentials grant type making backend/server API calls
- Oauth is a framework with exclusive authorization server API that generates access token to further allow access to inetract with Course Details API
- Front end API(User) makes call to auth server asking for access. Server will not provide access to all requests, hence to restrict/ avoid leakage it uses any of the 3 types to provide grant. 1. Client Credentials (widely used) 2. Password(widely used) 3. Authorization code
- I have used Client credentials grant type API in my automation code. It uses 2 parameters - client id and client secret in Form data. If validation is successful, access token is provided.
- In Password grant type, username and password is required in Form Data
- In the script, access token is stored as a string from jsonpath object parsed from response. Then it is passed in the Get request.
- Usually access token is passed via form data(so as to not expose critical information in URL) but here the api was developed to pass access token via query parameter
- Configured to run with Junit

If you have any questions, please contact me on neenyk18@gmail.com
