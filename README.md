# 🔐 21 Savage Fan Site — Authentication & Message Board

### Full-Stack Node.js Application

## About the Project

This is a full-stack message board application I worked on to practice user authentication, working with databases, and connecting the front end to the back end.

I started with an authentication boilerplate and customized it into a 21 Savage fan site where users can create accounts, log in, and post messages.

The goal was to get more comfortable understanding how authentication works and how user-generated information gets saved and displayed.

## Features

- **User Authentication:** Sign up and log in using an email and password.
- **Protected Profile:** Access the message board after logging in.
- **Create Messages:** Submit a message through a form.
- **View Messages:** Display messages stored in MongoDB.
- **Like and Dislike:** Use thumbs-up and thumbs-down buttons to interact with posts.
- **Delete Messages:** Remove posts from the message board.
- **Logout:** End the user session.

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Bootstrap
- Node.js
- Express.js
- EJS
- MongoDB and Mongoose
- Passport.js

## How It Works

1. A user visits the fan site and chooses Login or Signup.
2. Passport.js handles the authentication process.
3. After logging in, the user can access the profile page.
4. Users can submit messages that are saved in MongoDB.
5. The page displays messages from the database.
6. JavaScript uses the Fetch API to send requests for likes, dislikes, and deletions.

## Getting Started

1. Clone the repository:

   `git clone https://github.com/KevSal227/savageauth.git`

2. Open the project directory:

   `cd savageauth`

3. Install dependencies:

   `npm install`

4. Configure a MongoDB connection using the project's database configuration.

5. Start the server:

   `node server.js`

6. Visit `http://localhost:8080`.

**Note:** This project uses older dependencies and may need compatibility updates to run on modern Node.js versions.

## What I Learned

This project helped me better understand:

- Setting up an Express.js server.
- Working with Passport.js for authentication.
- Creating protected routes.
- Using sessions to keep users logged in.
- Saving and retrieving information with MongoDB.
- Handling GET, POST, PUT, and DELETE requests.
- Using the Fetch API to communicate with the back end.
- Displaying database information dynamically using EJS.

One of the biggest things I practiced was understanding how authentication and database operations work together in the same application.

## Current Limitations

This is a bootcamp learning project, and there are still improvements I would make:

- Fix the dislike logic so it updates a separate negative-vote counter.
- Use MongoDB ObjectIds to identify messages instead of matching their text.
- Restrict message modifications to authorized users.
- Avoid displaying stored password hashes on the profile page.
- Improve validation, error handling, and session security.
- Update older dependencies.

## Acknowledgments

The authentication structure was adapted from a Scotch.io authentication tutorial. I customized it by adding message-board functionality and interactions with MongoDB.
