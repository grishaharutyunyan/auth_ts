Login Registration 

Description

This project is a Node.js application built with Express.js. It provides a RESTful API for authentication and user management, utilizing MongoDB for database storage. The project incorporates various middleware for handling sessions, CORS, body parsing, and more. The application also leverages Passport.js for authentication.

Features

RESTful API for authentication and user management
Session management with express-session
Cross-Origin Resource Sharing (CORS) support
Body parsing using body-parser and express.json
Cookie parsing with cookie-parser
Authentication with Passport.js
Error handling middleware
Connection to MongoDB database
Requirements

Node.js (version 14.x or higher)
MongoDB instance
Environment variables configuration
Installation

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/your-project.git
cd your-project
Install dependencies:

bash
Copy code
npm install
Create a .env file in the root directory and add the following variables:

env
Copy code
FRONT_END=your_frontend_url
PORT=your_preferred_port
SESSION_SECRET=your_session_secret
MONGO_URI=your_mongodb_uri
Start the server:

bash
Copy code
npm start
Usage

The server will start on the port specified in the .env file. The following endpoints are available:

Authentication Routes
POST /api/auth/login - Log in a user
POST /api/auth/register - Register a new user
POST /api/auth/logout - Log out a user
User Routes
GET /api/user/profile - Get the logged-in user's profile
PUT /api/user/profile - Update the logged-in user's profile
Middleware

CORS: Allows cross-origin requests from the specified front-end URL.
express-session: Manages user sessions with a secret key.
passport: Initializes Passport.js for handling authentication.
body-parser: Parses incoming request bodies in a middleware before your handlers, available# auth_ts
Auth with Typescript
