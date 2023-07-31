# Blog Post API

This API is developed using TypeScript, Express.js, and MongoDB.

## Authentication

The API utilizes JSON Web Tokens (JWT) for user authentication. Upon successful registration, users receive a JWT token, which is used to authenticate subsequent requests. Users need to include the token in the authorization header for accessing protected routes, such as creating blog posts.

## Features

1. **User Registration**: Users can create their accounts by providing a unique username and password. Passwords are hashed before storage in the database for security.

2. **User Login**: Registered users can log in to the system using their credentials. Upon successful login, the API issues a JWT token to the user.

3. **Protected Routes**: Certain API routes, like creating blog posts, are protected and require user authentication. Users need to include their JWT token in the authorization header to access these routes.

4. **Create Blog Posts**: Authenticated users can create new blog posts, providing the title and content of the post.

## Technologies Used

- TypeScript: Provides type safety and improved tooling for JavaScript development.
- Express.js: A fast and flexible web application framework for building robust APIs.
- MongoDB: A NoSQL database used for storing user data and blog posts.
- JSON Web Tokens (JWT): A secure method for user authentication and authorization.

## Getting Started

To run the API locally:

1. Clone the repository.
2. Install dependencies using `npm install`.
3. Set up your MongoDB connection string in the `.env` file.
4. Run the API using `npm start`.
5. Access the API at `http://localhost:3000`.
