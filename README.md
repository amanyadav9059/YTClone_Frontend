
# YouTube Clone MERN Application

This repository contains a full-stack YouTube clone application built using the MERN stack. The project is split into two main parts: the Frontend (built with React) and the Backend (built with Node.js, Express, and MongoDB). This combined README provides an overview, setup instructions, and usage details for the entire application.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation and Setup](#installation-and-setup)
  - [Frontend Setup](#frontend-setup)
  - [Backend Setup](#backend-setup)
- [Running the Application](#running-the-application)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Overview

The YouTube Clone MERN Application is a capstone project that mimics the core functionalities of YouTube. Users can view video content, search and filter videos, watch videos on a dedicated player page, and interact with features like comments and channel management. Authentication is handled using JWT to secure protected routes and user data.

---

## Features

- Home Page
  - Custom YouTube-style header and sidebar.
  - Grid layout displaying video thumbnails along with titles, channel names, and view counts.
  - Filter buttons and search functionality to easily find videos by title and category.
- User Authentication
  - User registration and login using JWT-based authentication.
  - A dynamic header that updates to show the logged-in user’s name.
- Video Player Page
  - Integrated video player with video details (title, description, channel info).
  - Interactive like/dislike buttons.
  - Comment section with add, edit, and delete functionalities.
- Channel Page
  - Channel creation for authenticated users.
  - Display of user-specific video lists.
  - Options for editing and deleting videos.
- Profile Page
  - Displays user name, channel name(if created) and buttons to navigate to channel and logout.
- Responsive Design
  - Fully responsive across mobile, tablet, and desktop devices.

---

## Tech Stack

- Frontend: React, React Router, Axios, SCSS
- Backend: Node.js, Express.js, MongoDB (Atlas)
- Authentication: JSON Web Tokens (JWT)
- Version Control: Git & GitHub

---

## Project Structure

/ (Root)
└── frontend/         # Contains the React application
    ├── public/
    ├── src/
    │   ├── components/   # Reusable UI components (e.g., VideoCard, Header, Sidebar)
    │   ├── pages/        # Main pages (login, signup, Channel, upload, profile)
    │   ├── App.js
    │   ├── index.js
    │   └── ...
    └── package.json


/ (Root) 
└── backend/          # Contains the Node.js and Express API
    ├── controllers/  # Request handlers for different routes (Auth, Videos, Channels, Comments)
    ├── models/       # Mongoose models for Users, Videos, Channels, Comments
    ├── routes/       # Express route definitions
    ├── config/       # Configuration files (database, JWT secret, etc.)
    ├── server.js     # Application entry point
    └── package.json




## Installation and Setup

### Frontend Setup

1. Clone the Frontend Repository

   cd YT_Clone-Frontend

2. Install Dependencies
   npm install

3. Configure Environment Variables
   - Create a `.env` file in the root of the project and add any necessary variables (e.g., API base URL).

4. Run the Development Server
   npm run dev

   The application should now be running on [http://localhost:5713](http://localhost:5713).

### Backend Setup

1. Clone the Backend Repository
   cd YT_clone-Backend

2. Install Dependencies

   npm install

3. Configure Environment Variables
   - Create a `.env` file in the backend directory. Typical variables include:
     - `PORT` (e.g., 5000)
     - `MONGO_URI` (your MongoDB connection string)
     - `JWT_SECRET` (a secret key for JWT signing)
  
4. Run the Server

   npm run dev
   The backend server will start on the specified port (default: [http://localhost:5000](http://localhost:5000)).

---

## Running the Application

Once both the frontend and backend servers are running, you can access the application by navigating to [http://localhost:5173] in your web browser. The frontend will make API calls to the backend server for authentication, video data, and more.

---

## Usage

- Authentication:
  - Use the sign-in button in the header to navigate to the login/register page.
  - Upon successful login, your username will be displayed in the header.
  
- Video Interaction:
  - Browse the home page to view available videos.
  - Use the search bar or filter buttons to find specific videos.
  - Click on a video to view its details on the video player page, where you can interact (like, dislike, comment).

- Channel Management:
  - Once authenticated, create your own channel.
  - Upload videos, and manage them via your channel page.

---

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create your feature branch: `git checkout -b feature/YourFeature`.
3. Commit your changes: `git commit -m 'Add new feature'`.
4. Push to the branch: `git push origin feature/YourFeature`.
5. Open a Pull Request.

For major changes, please open an issue first to discuss what you would like to change.

---
## Acknowledgements

- Built as a capstone project to enhance full-stack development skills using the MERN stack.
- Special thanks to Internshala, all contributors and the open-source community.

---

