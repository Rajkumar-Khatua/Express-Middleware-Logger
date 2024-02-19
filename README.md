# Express Middleware Logger

This Express application includes a middleware function that logs the request method, URL, access token (if provided), and timestamp for every request to the server. The middleware is applied globally to all routes in the Express application.

## Requirements

- Node.js
- Express
- Nodemon (optional)
- MongoDB instance for database storage (optional)

## Installation

1. Clone this repository to your local machine.
2. Run `npm install` to install the required dependencies.
3. Run `npm start` to start the server.

## Usage

Once the server is running, you can send HTTP requests to the provided routes. The middleware will log each request's method, URL, and access token (if provided) to the console in the specified format.

### Routes

- `GET /users` - Retrieve all users
- `POST /users` - Create a new user
- `GET /users/:id` - Retrieve a single user by ID
- `PUT /users/:id` - Update a user by ID
- `DELETE /users/:id` - Delete a user by ID

## Logging Format

The middleware logs the request method, URL, access token (if provided), and timestamp for every request to the server. The log is formatted as follows:

```bash
[Timestamp] Method: URL, AccessToken: "accessToken"
```

if no access token is provided, the log will be formatted as follows:

```bash
[Timestamp] Method: URL
```

## Dependencies

- express: Web framework for Node.js
- mongoose: MongoDB object modeling tool for Node.js
- dotenv: Loads environment variables from a .env file

## Author

Rajkumar Khatua
