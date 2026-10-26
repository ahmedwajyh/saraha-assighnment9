# Saraha App

## Project Overview

Saraha App is a backend application built with Node.js and Express.js. It allows users to create accounts, log in, manage their profiles, and share their profiles with others.

## Features

* User Registration and Login.
* Google Authentication.
* Password Hashing.
* JWT Authentication.
* Access and Refresh Tokens.
* User Profile Management.
* Share User Profile.
* Update User Information.
* Update Password.
* File Uploads Using Multer.
* MongoDB Database Integration.
* Redis Integration.

## Technologies Used

* Node.js
* Express.js
* MongoDB
* Mongoose
* Redis
* JSON Web Token (JWT)
* Bcrypt
* Multer
* Joi
* Google Auth Library

## Installation

1. Clone the repository:

   ```bash
   git clone YOUR_REPOSITORY_URL
   ```

2. Navigate to the project directory:

   ```bash
   cd saraha-application
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Configure your environment variables in:

   * `config/.env.development`
   * `config/.env.production`

5. Start the development server:

   ```bash
   npm run start:dev
   ```

## API Endpoints

| Method | Endpoint                  | Description          |
| ------ | ------------------------- | -------------------- |
| POST   | `/user/signup`            | Register a new user  |
| POST   | `/user/signup/gmail`      | Google sign-up       |
| POST   | `/user/login`             | User login           |
| POST   | `/user/refresh-token`     | Refresh access token |
| GET    | `/user/profile`           | Get user profile     |
| GET    | `/user/share-profile/:id` | Share user profile   |
| PATCH  | `/user/update-profile`    | Update user profile  |
| PATCH  | `/user/update-password`   | Update password      |
| PATCH  | `/user/logout`            | User logout          |

## Database

The application uses MongoDB to store user data and Redis for caching and managing temporary data.

## File Uploads

Multer is used to upload user profile images and other attachments.

## Security

* Passwords are hashed before storage.
* JWT is used for authentication.
* Environment variables are excluded from GitHub.
* Sensitive credentials should never be committed to the repository.

## Environment Variables

Create your own environment files locally. Do not upload `.env` files to GitHub.

## Future Improvements

* Email Sending.
* Email OTP Verification.
* Store OTPs in Redis with an expiration time (TTL).

## Author

Ahmed Wageeh
