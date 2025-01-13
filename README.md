# User Authentication System

This project is a user authentication system built with React on the frontend, Node.js on the backend, and MongoDB for database storage. It supports registration with email confirmation, login with email confirmation, and password reset via email.

## Features

- **User Registration**:  
  Users can register for an account. A confirmation email is sent to verify their email address before activating the account.

- **Login**:  
  Users can log in using their email and password. Email confirmation is required before login.

- **Password Reset**:  
  Users can reset their password by requesting a verification code, sent to their email, and then entering the code and a new password.

## Getting Started

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

### Prerequisites

Ensure the following is installed:

- Node.js
- npm (Node Package Manager)

---

### Installation

#### Frontend Setup

1. Clone the repository:  
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. Install frontend dependencies:  
   ```bash
   npm install
   ```

3. Start the frontend development server:  
   ```bash
   npm start
   ```

   Open [http://localhost:3000](http://localhost:3000) to view the app in your browser.

#### Backend Setup

1. Configure environment variables:  
   Create a `.env` file in the backend directory with the following information:
   - Your MongoDB connection string
   - Credentials for an email service to send confirmation codes

   Example `.env` file:
   ```env
   MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/<database>?retryWrites=true&w=majority
   PORT=5001
   JWT_SECRET=your_jwt_secret
   EMAIL_HOST=smtp.example.com
   EMAIL_PORT=587
   EMAIL_USER=your_email@example.com
   EMAIL_PASS=your_email_password
   ```

2. Start the backend server:  
   ```bash
   node server.js
   ```

   The backend should now be running on [http://localhost:5001](http://localhost:5001) or the port specified in your `.env` file.

---

## Available Scripts (Frontend)

In the project directory, you can run:

### `npm start`

Runs the app in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

### `npm test`

Launches the test runner in the interactive watch mode.

### `npm run build`

Builds the app for production to the `build` folder.

---

## Learn More

- To learn React, check out the [React documentation](https://reactjs.org/).  
- For backend setup and API integration, refer to the documentation for Node.js and Express.

--- 

