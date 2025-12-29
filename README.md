# Linkidin - LinkedIn Clone

A full-stack social networking platform built with Node.js, Express, MongoDB, and React.

## Features

- **User Authentication**: Secure JWT-based authentication with password hashing
- **User Profiles**: Create and manage professional profiles with experience, education, and skills
- **Posts & Feed**: Share updates, images, and engage with other professionals
- **Connections**: Build your professional network by connecting with other users
- **Comments & Likes**: Interact with posts through comments and likes
- **Search**: Find and connect with professionals

## Project Structure

```
linkidin/
├── backend/              # Node.js + Express backend
│   ├── models/          # MongoDB schemas
│   │   ├── User.js      # User model with profile information
│   │   └── Post.js      # Post model for feed updates
│   ├── middleware/      # Express middleware
│   │   └── auth.js      # JWT authentication middleware
│   ├── routes/          # API routes (to be created)
│   ├── controllers/     # Business logic (to be created)
│   ├── server.js        # Express server setup
│   ├── package.json     # Node.js dependencies
│   └── .env.example     # Environment variables template
├── frontend/            # React frontend (to be created)
└── README.md           # This file
```

## Tech Stack

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling
- **JWT** - JSON Web Token authentication
- **Bcryptjs** - Password hashing

### Frontend (Planned)
- **React** - UI library
- **Redux** - State management
- **Axios** - HTTP client
- **Tailwind CSS** - Styling

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file based on `.env.example`:
```bash
PORT=5000
MONGODB_URI=mongodb://localhost:27017/linkidin
JWT_SECRET=your_secret_key_here
NODE_ENV=development
```

4. Start the server:
```bash
npm run dev  # For development with nodemon
# or
npm start    # For production
```

The backend will be running at `http://localhost:5000`

### API Endpoints

#### Health Check
- `GET /api/health` - Check if the server is running

#### Users (To be implemented)
- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login user
- `GET /api/users/:id` - Get user profile
- `PUT /api/users/:id` - Update user profile

#### Posts (To be implemented)
- `GET /api/posts` - Get feed
- `POST /api/posts` - Create a post
- `GET /api/posts/:id` - Get single post
- `DELETE /api/posts/:id` - Delete post

#### Connections (To be implemented)
- `GET /api/connections` - Get user connections
- `POST /api/connections/:userId` - Add connection
- `DELETE /api/connections/:userId` - Remove connection

## Frontend Development

Frontend setup instructions will be added as development progresses.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Author

Kritheeck - CSE Student at Meenakshi Sundararajan Engineering College
