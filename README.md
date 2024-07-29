This project demonstrate managing an API by making server side REST requests. These are GET, POST, PUT, PATCH, DELETE API requests used for API management.

Function of each REST request:

- GET: Retrieve data from the server.
- POST: Submit new data to the server.
- PUT: Update existing data on the server.
- PATCH: Partially update existing data on the server.
- DELETE: Remove data from the server.

Technology used in project:

1. Express: Web framework for Node.js to create and manage the server.
2. Axios: HTTP client for making API requests.
3. Body-Parser: Middleware to parse URL-encoded request bodies.
4. Bearer Token Authentication: Using a bearer token for secure API requests.
5. EJS: Templating engine for rendering views.
6. CSS: For basic frontend styling.
7. Node.js: JavaScript runtime for executing server-side code.

You will need a Bearer Token to use this project. To have a Bearer Token you will need to register and use your username and password to generate a Bearer Token. This will need to be done with Postman.

Register:

- Need to register via Postman

  POST https://secrets-api.appbrewery.com/register
  Request Body:
  {
  "username": "jackbauer",
  "password": "IAmTheBest"
  }

Bearer Token:

- Need to create Bearer Token using Postman
  POST https://secrets-api.appbrewery.com/get-auth-token

Request Body (must be the same as your username & password for when you registered previously):
{
"username": "jackbauer",
"password": "IAmTheBest"
}

How to run (ensure Node is installed on PC):

1. Ensure in the correct directory
2. Install NPM packages - npm i
3. Run code: node index.js
4. Now go to your web browsing application (Google Chrome, Safari, Firefox, Opera) and type in "localhost:3000/"
5. Use the project!
