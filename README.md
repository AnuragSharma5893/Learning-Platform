# Edtech Project

```markdown
# Learning Platform - Full Stack Application (MERN)

## Introduction
Welcome to the EdTech Platform, a full-stack educational technology application built using the MERN (MongoDB, Express.js, React, Node.js) stack. This platform provides a comprehensive solution for online education, enabling educators to create and manage courses, and allowing students to enroll in and complete courses.

## Features
- **User Authentication:** Secure user registration and login using JWT.
- **Role-Based Access Control:** Different access levels for administrators, educators, and students.
- **Course Management:** Create, update, delete, and view courses.
- **Lesson Management:** Add, edit, delete, and view lessons within courses.
- **Enrollment:** Students can enroll in courses and track their progress.
- **Discussion Forums:** Enable communication between students and educators.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Tech Stack
- **Frontend:**
  - React

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (Mongoose for ORM)
  - JWT (for authentication)

- **Development Tools:**
  - Webpack (module bundler)
  - Babel (JavaScript compiler)
  - Prettier (code formatting)

## Installation
### Prerequisites
- Node.js (>=14.x)
- MongoDB (>=4.x)

### Clone the Repository
```bash
git clone https://github.com/AnuragSharma5893/Learning-Platform.git
cd Learning-Project
```

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables:
   Create a `.env` file in the backend directory and add the following:
   ```plaintext
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the frontend development server:
   ```bash
   npm start
   ```

## Usage
1. Open your browser and navigate to `http://localhost:3000`.
2. Register as a new user or login with existing credentials.
3. Explore the platform's features by creating courses, enrolling, participating in forums, etc.

## Project Structure
```plaintext
Learning-platform/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   ├── .env
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── utils/
│   │   ├── App.js
│   │   ├── index.js
│   ├── public/
│   ├── .env
│   └── package.json
│
└── README.md
```

## API Documentation
### Authentication
- **POST /api/auth/register:** Register a new user.
- **POST /api/auth/login:** Log in a user and return a JWT.

### Courses
- **GET /api/courses:** Get all courses.
- **POST /api/courses:** Create a new course.
- **GET /api/courses/:id:** Get a single course by ID.
- **PUT /api/courses/:id:** Update a course by ID.
- **DELETE /api/courses/:id:** Delete a course by ID.

### Lessons
- **GET /api/courses/:courseId/lessons:** Get all lessons in a course.
- **POST /api/courses/:courseId/lessons:** Add a new lesson to a course.
- **GET /api/lessons/:id:** Get a single lesson by ID.
- **PUT /api/lessons/:id:** Update a lesson by ID.
- **DELETE /api/lessons/:id:** Delete a lesson by ID.

### Enrollments
- **POST /api/courses/:courseId/enroll:** Enroll in a course.
- **GET /api/users/:userId/enrollments:** Get all enrollments for a user.

## Contributing
We welcome contributions to improve the EdTech Platform. Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries or feedback, please contact:
- **Name:** Anurag Sharma
- **Email:** anuragsharma58693 [at] gmail [dot] com
- **GitHub:** github.com/AnuragSharma5893
```
