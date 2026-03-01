Todo App Backend API Documentation

Project Overview
This backend API is developed for the React Native Todo Application. It is built using Node.js, Express.js, MongoDB (MongoDB Atlas), and Mongoose. The API handles user authentication and task management with JWT-based authorization.

Tech Stack
  •	Node.js
  •	Express.js
  •	MongoDB Atlas
  •	Mongoose
  •	JWT (JSON Web Token)
  •	bcryptjs (Password Hashing)
  •	dotenv
  
Features Implemented
  •	User Registration
  •	User Login Authentication
  •	Password Hashing using bcrypt
  •	JWT-based Authorization
  •	Create Task
  •	View Tasks
  •	Update Task (Mark as Complete)
  •	Delete Task
  •	MongoDB Cloud Database Integration
  •	Backend Deployment on Render
  
Project Structure
  controllers/
  middleware/
  models/
  routes/
  server.js
  package.json
  package-lock.json
  .gitignore
  README.md
  
Installation & Setup
  1. Clone Repository
  git clone https://github.com/vishwasmagar10/TodoApp.git
  cd TodoApp
  2. Install Dependencies
  npm install
  3. Create .env File
  PORT=1000
  MONGO_URI=your_mongodb_connection_string
  JWT_SECRET=your_secret_key
  4. Run the Server
  npm start

Server will run at:
http://localhost:1000

**API Endpoints**

Authentication Routes
POST /api/auth/register - Register new user
POST /api/auth/login - Login user
Task Routes (Protected)
POST /api/tasks - Create new task
GET /api/tasks - Get all tasks
PUT /api/tasks/:id - Update task
DELETE /api/tasks/:id - Delete task

Authentication Flow
  1.	User registers with email and password.
  2.	Password is hashed using bcrypt.
  3.	On login, JWT token is generated.
  4.	Token must be sent in request headers as: Authorization: Bearer <token>

Environment Variables
  •	PORT - Server port
  •	MONGO_URI - MongoDB Atlas connection string
  •	JWT_SECRET - Secret key for JWT

  
Developer
Vishwas Magar
GitHub: https://github.com/vishwasmagar10
