# YouTube Clone

A feature-rich YouTube clone built using modern web development technologies like React, Node.js, Express.js, and MongoDB. The application allows users to watch, upload, and interact with video content.

## Table of Contents

1. [Features](#features)
2. [Technologies Used](#technologies-used)
3. [Installation and Setup](#installation-and-setup)
4. [Usage](#usage)
5. [Sample Data](#sample-data)
6. [API Endpoints](#api-endpoints)
7. [Contributing](#contributing)


## Features

- **User Authentication**
  - Sign up, log in, and secure authentication using JSON Web Tokens (JWT).
  - Google Form integration for login and registration.
- **Search and Filters**
  - Search videos by title and filter them by category.
- **Video Management**
  - Watch videos with titles, descriptions, and channel details.
  - Like/dislike videos and add/edit/delete comments.
- **Channel Management**
  - Create, update, and delete your own channels.
  - Manage videos within channels.
- **Responsive Design**
  - Fully responsive across mobile, tablet, and desktop devices.



## Technologies Used

- **Frontend**: React, React Router, Axios, TailwindCSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (MongoDB Atlas or local instance)
- **Authentication**: JSON Web Tokens (JWT)
- **Version Control**: Git


## Installation and Setup


1. Navigate to the project directory:
   ```bash
   cd youtube-clone
   ```
2. Install dependencies for the backend:
   ```bash
   cd server
   npm install
   ```
3. Install dependencies for the frontend:
   ```bash
   cd ../client
   npm install
   ```
4. Run the backend:
   ```bash
   cd server
   npm start
   ```
5. Run the frontend:
   ```bash
   cd ../client
   npm start
   ```
6. Open the app in your browser:
   ```
   http://localhost:4000


## Usage

- Sign up or log in to your account.
- Search for videos or filter them by categories.
- Watch videos, like/dislike them, and leave comments.
- Create your own channel and upload videos.
- Edit or delete videos from your channel.



## Sample Data

**Sample Channel Data**:
```json
{
  "channelId": "channel01",
  "channelName": "Code with John",
  "owner": "user01",
  "description": "Coding tutorials and tech reviews by John Doe.",
  "subscribers": 5200,
  "videos": ["video01", "video02"]
}


## API Endpoints

### User Authentication
- `POST /auth/signUp` - Register a new user.
- `POST /auth/login` - Login user and return JWT.
- `POST /auth/logout` - Logout user and clear JWT.

### Video Management
- `POST /api/video` - Upload a video.
- `GET /api/allVideo` - Get all videos.
- `GET /api/getVideoById/:id` - Get a video by Id.
- `GET /api/:userId/channel` - Get all videos uploaded by an user.
- `GET /api/videos/search` - Search a video.
