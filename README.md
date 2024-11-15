
# Online Complaint Management System

## Overview

The **Online Complaint Management System (OCMS)** is a web-based application designed to streamline the process of submitting, tracking, and resolving complaints. It provides a platform for users to file complaints, and for administrators to manage and resolve these complaints efficiently. The system aims to ensure better customer service, transparency, and responsiveness.

### Key Features:
- **User Authentication**: Allows users to register, log in, and track their complaints.
- **Complaint Submission**: Users can submit complaints with relevant details (e.g., type, description, and priority).
- **Complaint Tracking**: Users can view the status of their complaints in real-time.
- **Admin Panel**: Administrators can view all complaints, assign them to appropriate departments or staff, and mark them as resolved.
- **Complaint Categorization**: Complaints can be categorized based on their nature (e.g., technical issues, customer service, etc.).
- **Notifications**: Users and administrators receive notifications regarding the status of complaints.
- **Search & Filter**: Users and admins can search and filter complaints based on criteria like status, date, priority, etc.

---

## Table of Contents

- [Installation](#installation)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Installation

To run the **Online Complaint Management System** locally, follow these steps:

### Prerequisites

1. Install [Node.js](https://nodejs.org/) (for backend) and [npm](https://www.npmjs.com/).
2. Install [MongoDB](https://www.mongodb.com/try/download/community) for the database (alternatively, you can use a cloud database like [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)).
3. Install [Git](https://git-scm.com/) for cloning the repository.

### Steps to Set Up:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/anthonysahayasudharson/Online-Complaint-Management-System.git
   cd Online-Complaint-Management-System
   ```

2. **Install Dependencies:**

   For the backend:

   ```bash
   cd backend
   npm install
   ```

   For the frontend (if separate):

   ```bash
   cd frontend
   npm install
   ```

3. **Set up the Database:**

   - Ensure MongoDB is running locally or configure MongoDB Atlas and update the `config.js` or `env` file with your MongoDB URI.
   - If you are using MongoDB locally, make sure the MongoDB server is running.

4. **Start the Application:**

   - For the backend:

     ```bash
     cd backend
     npm start
     ```

   - For the frontend:

     ```bash
     cd frontend
     npm start
     ```

   The backend will run on `http://localhost:5000` (or whichever port you configure), and the frontend will run on `http://localhost:3000`.

---

## Technologies Used

- **Frontend**:
  - HTML5, CSS3, JavaScript
  - React.js (for dynamic UI)
  - Axios (for HTTP requests)

- **Backend**:
  - Node.js
  - Express.js (for RESTful API)
  - MongoDB (for database management)
  - JWT (JSON Web Tokens) for authentication
  - Bcrypt.js (for password hashing)

- **Other Tools**:
  - Nodemailer (for sending email notifications)
  - Multer (for file uploads, if needed)
  - Mongoose (for interacting with MongoDB)

---

## Features

1. **User Management**:
   - User registration with email verification.
   - Login/Logout functionality.
   - Password reset via email.

2. **Complaint Management**:
   - User-submitted complaints can be tracked with status updates (e.g., Pending, In Progress, Resolved).
   - Admins can view, filter, and search complaints by status, date, and category.
   - Complaints are assigned to relevant departments for resolution.

3. **Complaint Categories**:
   - Complaints are categorized by type (e.g., Service Issue, Technical Problem, Feedback, etc.).
   - Each category may have different response times and resolution paths.

4. **Notifications**:
   - Users and admins receive email and in-app notifications about new complaints, updates, and resolutions.

5. **Admin Panel**:
   - Admins have the ability to assign complaints to specific staff members.
   - Admins can mark complaints as resolved or escalated.

6. **Responsive UI**:
   - The system is designed to work on both desktop and mobile devices.

7. **Security**:
   - Passwords are hashed for security.
   - JWT is used for session management and API security.

---

## Usage

1. **For Users**:
   - Navigate to the **complaint submission page** after logging in.
   - Fill out the complaint form with the required information.
   - You can track the status of your complaint from your dashboard.

2. **For Admins**:
   - Admins can log in to the admin dashboard to manage complaints.
   - Admins can filter complaints by category, status, and priority.
   - They can assign complaints to staff and mark them as resolved.

---

## Folder Structure

The project follows a common structure for full-stack applications.

```
/Online-Complaint-Management-System
├── /backend
│   ├── /models         # MongoDB models
│   ├── /routes         # Express routes (API endpoints)
│   ├── /controllers    # Logic for handling requests
│   ├── /config         # Configuration files (database, JWT, etc.)
│   └── /middleware     # Middleware for authentication, error handling, etc.
│
├── /frontend
│   ├── /src
│   │   ├── /components # React components
│   │   ├── /pages      # React pages (e.g., Dashboard, Login)
│   │   ├── /utils      # Utility functions and helpers
│   │   └── /context    # Context API for global state management
│   └── package.json    # Frontend dependencies
│
└── README.md           # This file
```

---

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes and commit (`git commit -am 'Add feature'`).
4. Push to your branch (`git push origin feature-name`).
5. Create a pull request.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

For any issues or inquiries, feel free to contact the project maintainer:

- **Name**: Anthony Sahayasudharson
- **Email**: [your-email@example.com]
- **GitHub**: [github.com/anthonysahayasudharson](https://github.com/anthonysahayasudharson)
