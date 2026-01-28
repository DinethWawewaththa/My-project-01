# 🏠 StayNest

**StayNest** is a web-based platform designed to help users easily find and manage boarding houses, rooms, and shared accommodations. It connects tenants with boarding house owners through a simple, secure, and user-friendly system.

> **Tagline:** Find your place. Feel at home.

---

## 📌 Problem Statement

Finding a safe, affordable, and suitable boarding house is often time-consuming and unreliable. Information is scattered, outdated, or incomplete, making it difficult for tenants and owners to connect efficiently.

StayNest solves this problem by providing a centralized platform where:
- Tenants can search and compare boarding houses
- Owners can list and manage their properties
- Admins can ensure listing quality and safety

---

## 🎯 Objectives

- Simplify boarding house discovery
- Provide transparent pricing and rules
- Allow owners to manage listings digitally
- Improve trust through reviews and verification
- Reduce scams and misinformation

---

## 👥 User Roles

### 1. Tenant
- Search boarding houses
- View details and photos
- Save favorite listings
- Contact owners
- Leave reviews and ratings

### 2. Owner (Landlord)
- Register and manage profile
- Add, edit, and delete listings
- Upload images
- Manage room availability
- Respond to tenant inquiries

### 3. Admin
- Approve or reject listings
- Manage users
- Monitor reviews and reports
- Maintain platform integrity

---

## 🌐 Key Features

- User authentication (JWT)
- Role-based access control
- Boarding house search & filters
- Image upload support
- Reviews and ratings system
- Location-based search
- Secure inquiry system

---

## 🧱 Tech Stack

### Frontend
- React.js
- React Router
- Axios
- Tailwind CSS / Material UI

### Backend
- Node.js
- Express.js
- JWT Authentication

### Database
- MongoDB
- Mongoose

### Other Tools
- Cloudinary (image uploads)
- Google Maps API (location)

---

## 🗂️ Project Structure
.................................................................................................

staynest/
│
├── client/ # React frontend
│ ├── src/
│ └── package.json
│
├── server/ # Node.js backend
│ ├── models/
│ ├── routes/
│ ├── controllers/
│ ├── middleware/
│ └── server.js
│
├── README.md
└── .env
...................................................................................................


---

## 🗄️ Database Models (Overview)

### User
- name
- email
- password
- role (tenant / owner / admin)
- phone
- verified

### BoardingHouse
- title
- description
- ownerId
- location
- price
- amenities
- rules
- images
- availability
- rating

### Review
- userId
- boardingHouseId
- rating
- comment

---

## 🚀 Installation & Setup

### Prerequisites
- Node.js
- MongoDB
- Git

### Steps

1. Clone the repository
```bash
git clone https://github.com/your-username/staynest.git

cd server
npm install
npm start

