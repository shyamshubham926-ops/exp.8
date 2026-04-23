# MERN Stack Authentication System

A complete production-ready authentication system built with Node.js, Express, MongoDB, and React (Vite).

## 🚀 Features
- **JWT Authentication**: Secure login with JSON Web Tokens.
- **Password Hashing**: Bcryptjs used for secure password storage.
- **Role-Based Access**: 
  - **User**: Can view their own profile.
  - **Admin**: Can view their profile and a list of all registered users.
- **Protected Routes**: Frontend routes protected by authentication status.
- **Form Validation**: Client and server-side validation for emails and passwords.

---

## 🛠️ Tech Stack
- **Frontend**: React, Vite, Axios, React Router.
- **Backend**: Node.js, Express, Mongoose.
- **Database**: MongoDB.

---

## ⚙️ Setup Instructions

### 1. Prerequisites
- Node.js installed.
- MongoDB running locally or a MongoDB Atlas URI.

### 2. Backend Setup
1. Navigate to the backend folder:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `backend/` directory:
   ```env
   PORT=5000
   MONGO_URI=mongodb://127.0.0.1:27017/auth_db
   JWT_SECRET=your_jwt_secret_key
   ```
4. Start the server:
   ```bash
   npm run dev
   ```

### 3. Frontend Setup
1. Navigate to the frontend folder:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

---

## 🧪 Testing with Dummy Data

Use the following credentials to test the system:

### **Admin User** (Can see all users)
- **Name**: Admin User
- **Email**: `admin@test.com`
- **Password**: `password123`
- **Role**: Admin

### **Regular User** (Can see only profile)
- **Name**: John Doe
- **Email**: `john@test.com`
- **Password**: `password123`
- **Role**: User

---

## 📂 Project Structure
```text
EXP-8-pro/
├── backend/
│   ├── config/db.js
│   ├── controllers/authController.js
│   ├── middleware/authMiddleware.js
│   ├── models/User.js
│   ├── routes/authRoutes.js
│   └── server.js
└── frontend/
    ├── src/
    │   ├── api.js
    │   ├── components/ProtectedRoute.jsx
    │   ├── pages/Dashboard.jsx, Login.jsx, Register.jsx
    │   └── App.jsx
```
