# Job Portal - Full Stack Application

A modern job portal built with the MERN stack (MongoDB, Express.js, React.js, Node.js) that connects job seekers with employers. Features include user authentication, job posting, application tracking, and profile management.

## 🌟 Features

### For Job Seekers
- Create and manage professional profiles
- Search and filter jobs by various parameters
- Apply to jobs with resume/cover letter
- Track application status
- Save favorite job listings
- Receive email notifications for application updates

### For Employers
- Post and manage job listings
- Review applications
- Search candidate profiles
- Schedule interviews
- Manage company profile
- Track posting analytics

## 🛠️ Tech Stack

### Frontend
- React.js 18.x
- Redux Toolkit for state management
- React Router v6 for navigation
- Tailwind CSS for styling
- Axios for API requests
- React Query for data fetching
- React Hook Form for form validation

### Backend
- Node.js 18.x
- Express.js 4.x
- MongoDB with Mongoose ODM
- JWT for authentication
- Bcrypt for password hashing
- Nodemailer for email notifications
- Express-validator for input validation

## 📋 Prerequisites

- Node.js (v18 or higher)
- MongoDB (v6 or higher)
- npm/yarn package manager
- Git

## 🚀 Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/job-portal.git
cd job-portal
```

2. Install backend dependencies
```bash
cd backend
npm install
```

3. Install frontend dependencies
```bash
cd frontend
npm install
```

4. Set up environment variables:

Create `.env` file in backend directory:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
SMTP_HOST=your_smtp_host
SMTP_PORT=your_smtp_port
SMTP_USER=your_smtp_username
SMTP_PASS=your_smtp_password
```

Create `.env` file in frontend directory:
```env
REACT_APP_API_URL=http://localhost:5000/api
```

5. Start the development servers

Backend:
```bash
cd backend
npm run dev
```

Frontend:
```bash
cd frontend
npm start
```

## 🔒 Authentication

The application uses JWT (JSON Web Tokens) for authentication:
- Access tokens expire after 1 hour
- Refresh tokens expire after 7 days
- Protected routes require valid JWT in Authorization header

## 🔑 API Endpoints

### Authentication
- POST /api/auth/register
- POST /api/auth/login
- POST /api/auth/refresh-token
- POST /api/auth/logout

### Jobs
- GET /api/jobs
- POST /api/jobs
- GET /api/jobs/:id
- PUT /api/jobs/:id
- DELETE /api/jobs/:id

### Applications
- POST /api/jobs/:id/apply
- GET /api/applications
- PUT /api/applications/:id

### User Profile
- GET /api/profile
- PUT /api/profile
- GET /api/profile/:id

## 📦 Deployment

1. Build the frontend:
```bash
cd frontend
npm run build
```

2. Set up production environment variables
3. Deploy backend to your preferred hosting service
4. Deploy frontend build to static hosting service

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

## 📝 License

This project is licensed under the MIT License - see the LICENSE.md file for details.

## 👥 Authors

- Your Name (@raghavkumar09)

## 🙏 Acknowledgments

- MongoDB for the database
- Express.js community
- React.js team
- Node.js community
