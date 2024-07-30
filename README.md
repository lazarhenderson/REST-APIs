# RESTful API Management Project

This project demonstrates managing an API by making server-side REST requests, including GET, POST, PUT, PATCH, and DELETE requests for API management.

## REST Request Functions

- **GET:** Retrieve data from the server.
- **POST:** Submit new data to the server.
- **PUT:** Update existing data on the server.
- **PATCH:** Partially update existing data on the server.
- **DELETE:** Remove data from the server.

## Technologies Used

1. **Express:** A web framework for Node.js to create and manage the server.
2. **Axios:** An HTTP client for making API requests.
3. **Body-Parser:** Middleware to parse URL-encoded request bodies.
4. **Bearer Token Authentication:** Secure API requests using a bearer token.
5. **EJS:** A templating engine for rendering views.
6. **CSS:** Basic frontend styling.
7. **Node.js:** A JavaScript runtime for executing server-side code.

## Authentication

You will need a Bearer Token to use this project. Follow these steps to register and generate a Bearer Token using Postman.

### Register

To register via Postman:

```http
POST https://secrets-api.appbrewery.com/register
```

**Request Body:**

```json
{
  "username": "jackbauer",
  "password": "IAmTheBest"
}
```

### Generate Bearer Token

Create a Bearer Token using Postman:

```http
POST https://secrets-api.appbrewery.com/get-auth-token
```

**Request Body (must match your registered username & password):**

```json
{
  "username": "jackbauer",
  "password": "IAmTheBest"
}
```

## How to Run

Ensure Node.js is installed on your PC. Then follow these steps:

1. Navigate to the project directory.
2. Install the required NPM packages:

   ```bash
   npm install
   ```

3. Run the code:

   ```bash
   node index.js
   ```

4. Open your web browser (Google Chrome, Safari, Firefox, Opera) and navigate to:

   ```http
   http://localhost:3000/
   ```

5. Use the project!
