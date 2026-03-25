# Secure Authentication API 🚀

Hey there! This is a backend infrastructure built specifically to handle secure user identity management. It runs on Express.js and MongoDB.

## What does it do?

It handles the most important parts of the user lifecycle with a simple, secure approach:
- **User Onboarding:** Safely register new users and hash their passwords (`POST /users/register`).

- **Identity Verification:** Authenticate returning users securely (`POST /users/login`).
- **Session Management:** Retrieve the currently authenticated user's profile using JSON Web Tokens (JWT) (`GET /users/me`).

## Features Under the Hood
- 🔐 **Argon2** for state-of-the-art password hashing.
- 🎫 **JWT (JSON Web Tokens)** for stateless, secure sessions.
- 🗄️ **MongoDB & Mongoose** for reliable data persistence.
- ⚡ **Vercel-Ready** configuration (`vercel.json`) allowing you to deploy the Express API in seconds.

## Getting Started Locally

1. **Install Dependencies:**
   ```bash
   npm install
   ```

2. **Environment Variables:**
   Make sure your `.env` file is set up with your `MONGO_URI` and `JWT_SECRET`.

3. **Run the Development Server:**
   ```bash
   npm run dev
   ```
   The API will start up on `localhost:3000`. 

## Deployment
This project is pre-configured for Vercel. To deploy:
1. Make sure the Vercel CLI is installed (`npm i -g vercel`).
2. Run `vercel` or let Vercel sync with your GitHub repository.
3. Your Express API is now live on the internet!
