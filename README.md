# Trackify - Main Documentation

Welcome to the main documentation for Trackify, a job application tracking system. This guide provides instructions on setting up and using the frontend and backend repositories of Trackify. Follow the steps below to get both the frontend and backend running together.

## Overview

Trackify is a full-stack application designed to help users manage their job applications efficiently. The application consists of two main parts:

- **Frontend**: Built with React, the frontend handles user interactions and displays job application data in a user-friendly interface.
- **Backend**: Built with Node.js and Express, the backend provides APIs for authentication, managing job applications, and data persistence using MongoDB.

## Prerequisites

- **Node.js** (v14+)
- **npm** (v6+) or **yarn** (v1.22+)
- **MongoDB**: Ensure you have MongoDB installed locally or access to a MongoDB Atlas cluster.

## Repository Links

- [Frontend Repository](#) - *([https://github.com/ananaymathur/Trackify-frontend](https://github.com/ananaymathur/Trackify-frontend))*
- [Backend Repository](#) - *([https://github.com/ananaymathur/Trackify-backend](https://github.com/ananaymathur/Trackify-backend))*

## Getting Started

### 1. Clone Both Repositories

Clone the frontend and backend repositories to your local machine.

```bash
# Clone the frontend repository
git clone https://github.com/yourusername/trackify-frontend.git
cd trackify-frontend
```

```bash
# Clone the backend repository in a separate directory
git clone https://github.com/yourusername/trackify-backend.git
cd trackify-backend
```

### 2. Setting Up the Backend

1. Navigate to the backend directory:

```bash
cd trackify-backend
```

2. Install the dependencies:

```bash
npm install
```

3. Set up environment variables by creating a .env file in the root directory:

```plaintext
PORT=5000
MONGO_URI=mongodb://localhost:27017/trackify
JWT_SECRET=your_jwt_secret
```

Replace MONGO_URI with your MongoDB connection string and set JWT_SECRET to a secure secret key for JWT signing.

4. Start the backend server:

```bash
npm start
```

The backend will run on http://localhost:4000 by default.

### 3. Setting Up the Frontend

1. Navigate to the frontend directory:

```bash
cd trackify-frontend
```

2. Install the dependencies:

```bash
npm install
```

3. Set up environment variables by creating a .env file in the root directory:

```plaintext
REACT_APP_API_URL=http://localhost:4000
```

Ensure the URL matches the backend URL you set up earlier.

4. Start the frontend application:

```bash
npm start
```

The frontend will run on http://localhost:3000 by default.

## Connecting Frontend and Backend

The frontend uses the REACT_APP_API_URL variable to connect to the backend API. Make sure both servers are running simultaneously, and that the URLs are correctly set in the .env files.
