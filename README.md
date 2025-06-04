
# Facebook Clone MVP

## Overview

This is a minimal social media web app clone built with React (frontend) and Express + MongoDB (backend). It supports user registration, login (with JWT authentication), posting, and viewing posts.

## Prerequisites

- Node.js (v16+ recommended)  
- MongoDB running locally or a MongoDB Atlas URI  
- npm (comes with Node.js)  

## Backend Setup

1. Unzip and open the `facebook_clone_backend` folder.

2. Create a `.env` file at the root with the following variables:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

3. Install dependencies and start the server:

```bash
npm install
npm start
```

The backend server will run on `http://localhost:5000`

## Frontend Setup

1. Unzip and open the `facebook_clone_frontend` folder.

2. Install dependencies:

```bash
npm install
```

3. Start the React development server:

```bash
npm start
```

The frontend will run on `http://localhost:3000`

## Usage

- Visit `http://localhost:3000/register` to create an account.  
- Login at `http://localhost:3000/login`.  
- After login, you’ll be redirected to the home page where you can create posts and see others' posts.  
- Logout using the button in the top-right.

## Notes

- Make sure your backend server is running before using the frontend.  
- API requests are hardcoded to `http://localhost:5000/api/`—update if hosting differently.  
- JWT token is stored in localStorage to persist login state.  
- You can extend features like profile avatars, likes, comments, and more!
