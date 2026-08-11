# 🎟️ Eventaura – Event Booking Web Application

Eventaura is a full-stack **Event Booking Web Application** built using the **MERN Stack (MongoDB, Express.js, React.js, Node.js)**.

The platform allows users to create an account, securely log in, browse available events, view event details, and book events. It also provides a user dashboard where users can view their booked events.

---

## 🚀 Features

* 🔐 User Registration & Login
* 🔑 JWT-based Authentication
* 📧 OTP Verification
* 🎫 Browse Available Events
* 📋 View Detailed Event Information
* 🎟️ Book Events
* 👤 User Dashboard
* 📚 View Previously Booked Events
* 🔒 Protected API Routes
* 🌐 RESTful API Architecture
* 📱 Responsive User Interface
* 🗄️ MongoDB Database Integration

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Vite
* React Router
* Axios
* React Icons
* CSS / Tailwind CSS

### Backend

* Node.js
* Express.js
* Mongoose
* JWT Authentication
* Nodemailer
* REST APIs

### Database

* MongoDB

### Development Tools

* Git & GitHub
* VS Code
* Postman

---

## 📂 Project Structure

```text
Eventaura/
│
├── client/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── utils/
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   └── vite.config.js
│
├── server/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── server.js
│   ├── package.json
│   └── .env
│
├── .gitignore
└── README.md
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd Eventaura
```

### 2. Install Frontend Dependencies

```bash
cd client
npm install
```

### 3. Install Backend Dependencies

Open another terminal:

```bash
cd server
npm install
```

---

## 🔐 Environment Variables

Create a `.env` file inside the `server` folder.

```env
PORT=5000
MONGO_URL=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

EMAIL_USER=your_email
EMAIL_PASS=your_email_app_password
```

> ⚠️ Never upload your `.env` file to GitHub. Make sure it is included in `.gitignore`.

---

## ▶️ Run the Application

### Start Backend

```bash
cd server
npm start
```

or, if using nodemon:

```bash
npm run dev
```

The backend will run on:

```text
http://localhost:5000
```

### Start Frontend

```bash
cd client
npm run dev
```

The frontend will normally run on:

```text
http://localhost:5173
```

---

## 🔗 API Endpoints

### Authentication

| Method | Endpoint               | Description         |
| ------ | ---------------------- | ------------------- |
| POST   | `/api/auth/register`   | Register a new user |
| POST   | `/api/auth/login`      | Login user          |
| POST   | `/api/auth/verify-otp` | Verify OTP          |

### Events

| Method | Endpoint          | Description     |
| ------ | ----------------- | --------------- |
| GET    | `/api/events`     | Get all events  |
| GET    | `/api/events/:id` | Get event by ID |
| POST   | `/api/events`     | Create an event |

### Bookings

| Method | Endpoint           | Description         |
| ------ | ------------------ | ------------------- |
| POST   | `/api/bookings`    | Book an event       |
| GET    | `/api/bookings/my` | Get user's bookings |

---

## 🔐 Authentication Flow

Eventaura uses **JWT (JSON Web Token)** for authentication.

```text
User
  │
  ├── Register
  │
  ▼
OTP Verification
  │
  ▼
Login
  │
  ▼
JWT Token
  │
  ▼
Protected API Requests
  │
  ▼
User Dashboard / Bookings
```

---

## 📸 Application Workflow

```text
Landing Page
     │
     ▼
Register / Login
     │
     ▼
Events Page
     │
     ▼
Select Event
     │
     ▼
Event Details
     │
     ▼
Book Event
     │
     ▼
User Dashboard
     │
     ▼
View Bookings
```

---

## 💡 Key Learning Outcomes

Through this project, I gained practical experience in:

* Building a full-stack MERN application
* Creating RESTful APIs using Express.js
* Connecting React with a Node.js backend
* Working with MongoDB and Mongoose
* Implementing JWT authentication
* Implementing OTP verification
* Protecting backend routes
* Managing API requests using Axios
* Using React Router for navigation
* Managing frontend and backend project structure
* Working with environment variables
* Using Git and GitHub for version control

---

## 🔮 Future Improvements

Some features that can be added in future versions:

* 💳 Online Payment Integration
* 📱 Improved Mobile Responsiveness
* 🔎 Event Search & Filtering
* 📍 Location-based Event Search
* ⭐ Event Reviews & Ratings
* ❤️ Favorite Events
* 🔔 Email Notifications
* 📊 Admin Dashboard
* 🎫 QR Code-based Event Tickets
* ☁️ Cloud Deployment

---

## 👨‍💻 Developer

**Nilesh Chudasama**

Full Stack Web Developer | MERN Stack

### Skills

```text
React.js | Node.js | Express.js | MongoDB
JavaScript | Python | Django | MySQL
REST APIs | Git | GitHub
```

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ on GitHub.

---

## 📄 License

This project is created for educational and portfolio purposes.
