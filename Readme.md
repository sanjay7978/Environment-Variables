# 🔐 Secrets Authentication App

<div align="center">

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Passport](https://img.shields.io/badge/Passport.js-34E27A?style=for-the-badge)
![bcrypt](https://img.shields.io/badge/bcrypt-FF6B6B?style=for-the-badge)
![EJS](https://img.shields.io/badge/EJS-8BC34A?style=for-the-badge)

### Secure Authentication System using Node.js, Express, PostgreSQL, Passport.js & bcrypt

A full-stack authentication application that demonstrates secure user registration, login, session management, password hashing, and protected routes.

</div>

---

## 📖 Overview

**Secrets Authentication App** is a learning-focused full-stack web application that implements industry-standard authentication practices.

Users can:

- Create an account
- Login securely
- Access protected pages
- Maintain authenticated sessions
- Logout safely

The application uses **bcrypt** for password hashing and **Passport.js** for authentication management, ensuring that user credentials are never stored in plain text.

---

## ✨ Features

### 🔑 Authentication

- User Registration
- User Login
- User Logout
- Session-Based Authentication
- Protected Routes

### 🔒 Security

- Password Hashing using bcrypt
- Secure Session Management
- Environment Variable Support
- Authentication Middleware

### 🗄 Database

- PostgreSQL Integration
- User Data Storage
- Persistent Authentication Data

### 🎨 Frontend

- Responsive UI with Bootstrap
- Server-Side Rendering using EJS
- Reusable Layout Components
- Clean and Minimal Design

---

## 🛠 Tech Stack

### Backend

- Node.js
- Express.js
- PostgreSQL
- Passport.js
- Passport Local Strategy
- Express Session
- bcrypt
- dotenv

### Frontend

- EJS
- Bootstrap 4
- CSS3

---

## 📂 Project Structure

```bash
.
├── public
│   └── css
│       └── styles.css
│
├── views
│   ├── partials
│   │   ├── header.ejs
│   │   └── footer.ejs
│   │
│   ├── home.ejs
│   ├── login.ejs
│   ├── register.ejs
│   └── secrets.ejs
│
├── package.json
├── package-lock.json
└── solution.js
```

---

## 🚀 Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/secrets-auth-app.git
cd secrets-auth-app
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Create Environment Variables

Create a `.env` file in the root directory:

```env
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_password
DB_NAME=secrets

SESSION_SECRET=your_super_secret_key
```

---

### 4️⃣ Setup PostgreSQL

Create a database:

```sql
CREATE DATABASE secrets;
```

Create a users table:

```sql
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    email VARCHAR(255) UNIQUE NOT NULL,
    password TEXT NOT NULL
);
```

---

### 5️⃣ Run the Application

```bash
node solution.js
```

or

```bash
npm start
```

For development:

```bash
npx nodemon solution.js
```

---

## 🌐 Application Flow

### User Registration

```text
User
   ↓
Register
   ↓
Password Hashed using bcrypt
   ↓
Stored in PostgreSQL
```

### User Login

```text
User
   ↓
Login
   ↓
Passport Authentication
   ↓
Session Created
   ↓
Access Granted
```

### Protected Route

```text
Authenticated User
   ↓
Protected Route
   ↓
Secrets Page
```

---

## 📸 Screens

### 🏠 Home Page

- Register
- Login

### 📝 Register Page

- Email Input
- Password Input

### 🔑 Login Page

- Email Input
- Password Input

### 🔒 Secrets Page

- Accessible only after successful login

---

## 🧠 What I Learned

This project helped me understand:

- Authentication vs Authorization
- Password Hashing
- Session Management
- Express Middleware
- PostgreSQL Integration
- Passport.js Authentication
- Environment Variables
- Secure Backend Development Practices

---

## 🔮 Future Improvements

- Google OAuth Authentication
- GitHub OAuth Authentication
- User Submitted Secrets
- Password Reset Feature
- Email Verification
- JWT Authentication
- Profile Management
- Docker Support
- Deployment on AWS / Render / Railway

---

## ⚙️ Dependencies

```json
{
  "bcrypt": "^5.1.1",
  "body-parser": "^1.20.2",
  "dotenv": "^16.3.1",
  "ejs": "^3.1.9",
  "express": "^4.18.2",
  "express-session": "^1.17.3",
  "passport": "^0.7.0",
  "passport-local": "^1.0.0",
  "pg": "^8.11.3"
}
```

---

## 🏆 Resume Highlights

### Secrets Authentication App

- Built a secure authentication system using Node.js, Express.js, PostgreSQL, Passport.js, and bcrypt.
- Implemented user registration, login, logout, session management, and protected routes.
- Applied password hashing and authentication best practices for enhanced security.
- Developed responsive server-rendered UI using EJS and Bootstrap.
- Integrated PostgreSQL for persistent user data storage.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

<div align="center">

⭐ If you found this project useful, consider giving it a star!

Made with ❤️ using Node.js & PostgreSQL

</div>