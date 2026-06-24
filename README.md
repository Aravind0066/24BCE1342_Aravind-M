# 🏋️ Gym Hub

A full-stack Gym Management System built using **Node.js, Express.js, MongoDB, and JavaScript**.

Gym Hub enables gym administrators to manage members, trainers, membership plans, workout programs, and enrollments through a centralized dashboard. The project demonstrates CRUD operations, REST APIs, MongoDB relationships using ObjectId references, and frontend-backend integration using the Fetch API.

---

## 🚀 Features

### Member Management

* Add Members
* View Members
* Delete Members
* Update Members (API Supported)

### Trainer Management

* Add Trainers
* View Trainers
* Delete Trainers
* Update Trainers (API Supported)

### Membership Plans

* Create Plans
* View Plans
* Delete Plans
* Update Plans (API Supported)

### Workout Programs

* Create Workout Programs
* Assign Trainers
* Trainer Dropdown Selection
* Display Trainer Information using Mongoose Populate
* Delete Programs

### Enrollment Management

* Enroll Members into Programs
* Link Members, Plans, and Programs
* View Enrollments
* Delete Enrollments

### Database Features

* MongoDB Relationships
* ObjectId References
* Mongoose Populate
* CRUD Operations

---

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### Backend

* Node.js v24.16.0
* Express.js v5.2.1

### Database

* MongoDB Community Server v8.3.2
* Mongoose v9.7.0

### Development Tools

* Visual Studio Code v1.124.2
* Postman v12.15.5
* MongoDB Compass v1.49.8
* Mongosh v2.8.3

---

## 📂 Project Structure

```bash
GymHub/
│
├── config/
│   └── db.js
│
├── models/
│   ├── Member.js
│   ├── Trainer.js
│   ├── MembershipPlan.js
│   ├── WorkoutProgram.js
│   └── Enrollment.js
│
├── routes/
│   ├── memberRoutes.js
│   ├── trainerRoutes.js
│   ├── membershipPlanRoutes.js
│   ├── workoutProgramRoutes.js
│   └── enrollmentRoutes.js
│
├── public/
│   ├── index.html
│   ├── styles.css
│   └── script.js
│
├── .env
├── app.js
├── package.json
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd GymHub
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Create a MongoDB Database

Create a database named:

```text
smartgymdb
```

using MongoDB Compass or MongoDB Shell.

---

## 🔑 Environment Variables

Create a `.env` file in the root directory.

```env
PORT=5000

MONGO_URI=mongodb://127.0.0.1:27017/smartgymdb
```

If using MongoDB Atlas:

```env
PORT=5000

MONGO_URI=your_mongodb_atlas_connection_string
```

---

## ▶️ Running the Project

Start the backend:

```bash
node app.js
```

Expected output:

```bash
Server running on port 5000
MongoDB Connected
```

Open:

```text
http://localhost:5000
```

in your browser.

---

## 🔗 API Endpoints

### Members

```http
GET    /members
POST   /members
PUT    /members/:id
DELETE /members/:id
```

### Trainers

```http
GET    /trainers
POST   /trainers
PUT    /trainers/:id
DELETE /trainers/:id
```

### Membership Plans

```http
GET    /plans
POST   /plans
PUT    /plans/:id
DELETE /plans/:id
```

### Workout Programs

```http
GET    /programs
POST   /programs
PUT    /programs/:id
DELETE /programs/:id
```

### Enrollments

```http
GET    /enrollments
POST   /enrollments
PUT    /enrollments/:id
DELETE /enrollments/:id
```

---

## 🗄️ Database Collections

### Member

```javascript
{
  name,
  email,
  phone,
  age
}
```

### Trainer

```javascript
{
  name,
  specialization,
  experience
}
```

### Membership Plan

```javascript
{
  planName,
  duration,
  price
}
```

### Workout Program

```javascript
{
  programName,
  duration,
  trainerId
}
```

### Enrollment

```javascript
{
  memberId,
  planId,
  programId,
  enrollmentDate
}

```

## 🔮 Future Enhancements

* Frontend Update Functionality
* Authentication & Authorization
* Role-Based Access Control
* Attendance Tracking
* Payment Integration
* Progress Analytics
* Email Notifications

---

## 📖 Learning Outcomes

This project demonstrates:

* REST API Development
* CRUD Operations
* MongoDB Relationships
* Mongoose Populate
* Frontend-Backend Integration
* Database Design
* Express.js Routing
* Full-Stack Application Development

---

## 📄 License

This project was developed for educational and learning purposes.
