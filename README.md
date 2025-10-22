# TaskFlow

A full-stack project management application built with a Node.js/Express backend and a React/TypeScript frontend, using MongoDB as the database.

## 🚀 Live Demo
- **Frontend**: https://project-management-delta-weld.vercel.app
- **Backend API**: https://project-management-server-uo61.onrender.com
Note: The backend is deployed on Render's free tier, which spins down after inactivity. The first request may take 30-50 seconds to wake up the server, but subsequent requests will be fast.


### Test Credentials
- **Email**: test@example.com
- **Password**: Test@123

📋 Features
✅ Implemented Core Features
1. User Authentication (JWT-based)
✅ User registration and login with email & password
✅ JWT-based authentication with secure token storage
✅ Password hashing using bcrypt
✅ Protected routes and API endpoints

2. Project Management
✅ Create, read, update, and delete projects
✅ View user-specific project list
✅ Project fields: title, description, status ("active", "completed")
✅ Responsive project dashboard

3. Task Management
✅ Tasks associated with projects
✅ Task fields: title, description, status ("todo", "in-progress", "done"), due date
✅ Full CRUD operations on tasks
✅ Filter tasks by status
✅ Task status updates with dropdown

4. Frontend Implementation
✅ Login and registration pages
✅ Dashboard with user's projects
✅ Project details page with associated tasks
✅ Add/edit forms for projects and tasks
✅ Responsive design with Tailwind CSS
✅ TypeScript throughout the application

5. Seed Data
✅ Seeder script with test user, projects, and tasks
✅ Easy setup for testing and development

🎯 Bonus Features Implemented
✅ Form Validation: React Hook Form with built-in validation
✅ State Management: React Context API for authentication state
✅ Responsive Design: Mobile-friendly interface with Tailwind CSS

🛠️ Technology Stack
Backend
Node.js with Express.js framework
MongoDB with Mongoose ODM
JWT for authentication
bcryptjs for password hashing
CORS enabled for cross-origin requests

Frontend
React 18 with TypeScript
Vite as build tool
React Router for navigation
React Hook Form for form handling
Tailwind CSS for styling
Axios for API calls
React Hot Toast for notifications



📦 Installation & Setup
Prerequisites
Node.js (v16 or higher)
MongoDB (local or Atlas)
npm

### Backend Setup
1. **Clone the repository**
```bash
git clone <repository-url>
cd project-management/backend

2.Install dependencies
npm install

3.Environment Configuration
Create a .env file in the backend directory (or rename .env.example to .env):

env
PORT=5001
MONGODB_URI=mongodb://localhost:27017/project_management
JWT_SECRET=your_jwt_secret_key_here
NODE_ENV=development
CORS_ORIGIN=http://localhost:5173

4.Start MongoDB (make sure MongoDB is running on your system)

5.Start the backend server
# Development
- `npm run dev` - Start development server with nodemon

# Production
- `npm start` - Start production server

##Seed data
- `npm run seed` - Populate database with sample data



Frontend Setup

1.Navigate to frontend directory in a new terminal
cd frontend

2.Install dependencies
npm install

3.Start the frontend development server
- `npm run dev` - Start development server


🗃️ Database Seeding
Run Seed Script
To populate the database with sample data:
cd backend
npm run seed

Seed Data Created
Test User:
Email: test@example.com
Password: Test@123

Sample Projects (2 projects):
Website Redesign
Mobile App Development

Sample Tasks (6 tasks total, 3 per project):
Various statuses: todo, in-progress, done
Realistic task titles and descriptions
Sample due dates


🚀 Deployment
Backend Deployment (Render)
Frontend Deployment (Vercel)


📁 Project Structure
project-management-tool/
├── backend/
│   ├── src/
│   │   ├── models/
│   │   │   ├── User.js
│   │   │   ├── Project.js
│   │   │   └── Task.js
│   │   ├── middleware/
│   │   │   └── auth.js
│   │   ├── routes/
│   │   │   ├── auth.js
│   │   │   ├── projects.js
│   │   │   └── tasks.js
│   │   ├── seeders/
│   │   │   └── seed.js
│   │   └── app.js
│   ├── package.json
|   ├── .env.example
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── components/
|   |   |   └── PrivateRoute.tsx
│   │   ├── pages/
│   │   │   ├── Login.tsx
│   │   │   ├── Register.tsx
│   │   │   ├── Dashboard.tsx
│   │   │   ├── ProjectDetail.tsx
│   │   │   ├── ProjectForm.tsx
│   │   │   └── TaskForm.tsx
│   │   ├── context/
│   │   │   └── AuthContext.tsx
│   │   ├── types/
│   │   │   └── index.ts
│   │   ├── utils/
│   │   │   └── api.ts
│   │   └── App.tsx
│   ├── package.json
│   ├── vite.config.ts
│   └── vercel.json
└── README.md


🔌 API Endpoints
Authentication
POST /api/auth/register - User registration
POST /api/auth/login - User login

Projects
GET /api/projects - Get user's projects
POST /api/projects - Create new project
GET /api/projects/:id - Get project details
PUT /api/projects/:id - Update project
DELETE /api/projects/:id - Delete project

Tasks
GET /api/tasks/project/:projectId - Get project tasks
POST /api/tasks - Create new task
PUT /api/tasks/:id - Update task
DELETE /api/tasks/:id - Delete task

⚠️ Known Limitations
1.No Real-time Updates: Changes don't reflect in real-time across multiple sessions
2.No File Uploads: Cannot attach files to projects or tasks
3.Basic Error Handling: Error messages could be more user-friendly
4.No Email Verification: User registration doesn't require email confirmation
5.No Password Reset: No functionality to reset forgotten passwords
6.No Advanced Filtering: Limited to basic status filtering for tasks
7.No User Roles: All users have the same permissions

🔮 Future Enhancements
Real-time collaboration with WebSockets
File uploads and attachments
Advanced search and filtering
User roles and permissions
Email notifications
Password reset functionality
Project sharing and collaboration
Calendar view for tasks
Data export functionality
Unit and integration tests


## ✅ Assignment Requirements Met

### Core Requirements (100%)
- ✅ **Node.js/Express Backend** - Complete REST API with JWT authentication
- ✅ **React + TypeScript Frontend** - Full TypeScript implementation
- ✅ **MongoDB Database** - With Mongoose ODM
- ✅ **User Authentication** - JWT-based with bcrypt password hashing
- ✅ **Project CRUD** - Create, read, update, delete projects
- ✅ **Task CRUD** - Tasks associated with projects with status filtering
- ✅ **Seed Script** - Populates database with test user, projects, and tasks

### Frontend Requirements
- ✅ Login/register pages with form validation
- ✅ Dashboard with project list
- ✅ Project details page with tasks
- ✅ Add/edit forms for projects and tasks
- ✅ Tailwind CSS styling
- ✅ TypeScript throughout

### Bonus Features Implemented
- ✅ Form validation with React Hook Form
- ✅ State management with React Context
- ✅ Responsive design
- ✅ TypeScript in both frontend and backend

🤝 Author
Siddhant Sharma 
* GitHub: [https://github.com/Siddhant7621]
* LinkedIn: [https://www.linkedin.com/in/siddhantsharma7621]




