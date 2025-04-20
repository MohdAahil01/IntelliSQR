#  IntelliSQR – Full Stack Authentication App

Welcome to **IntelliSQR** – a modern full-stack authentication system built as part of the IntelliSQR internship assignment. This project includes a secure Express + Prisma backend and a responsive React + Tailwind frontend with form validation and API integration.

---

##  Project Structure

IntelliSQR/
├── frontend/      # React + Vite + Tailwind
├── backend/       # Express + TypeScript + Prisma
├── README.md      # This file

---

## 🚀 Tech Stack Overview

### 🔹 Frontend
- React + TypeScript
- Vite
- Tailwind CSS
- React Hook Form + Zod (validation)
- Axios (API requests)
- React Router DOM
- React Query

### 🔹 Backend
- Node.js + Express
- TypeScript
- Prisma ORM
- SQLite (can upgrade to PostgreSQL)
- Bcrypt (password hashing)
- JWT (optional)
- CORS, error handling middleware

---

## ⚙️ Setup Instructions

### 🔧 Prerequisites

- Node.js installed (v18 or later recommended)
- Git installed

---

### 🖥️ Backend Setup

```bash
cd backend
npm install


### 1. Create a .env file using the provided .env.example:

DATABASE_URL="file:./dev.db"
JWT_SECRET=your_jwt_secret

### 2. Initialize Prisma:

npx prisma migrate dev --name init

### 3. Start the backend:

npm run dev
Runs at: http://localhost:3005

## You can test the DB visually:

npx prisma studio



# Frontend Setup 

```bash 
cd frontend
npm install

1.	Create a .env file using the provided .env.example:
   
VITE_API_URL=http://localhost:3005/api

2.	Run the frontend:

npm run dev
Runs at: http://localhost:5173


## App Features
	•	User registration and login
	•	Form validation using Zod
	•	Proper error handling (e.g. wrong password, user exists)
	•	Passwords securely hashed
	•	Fully responsive UI with Tailwind CSS
	•	API tested via curl, Postman, and UI

# Video Demonstration

📌 A short video has been recorded to demonstrate:
	•	✅ Registering a user
	•	✅ Logging in successfully
	•	✅ UI validation (e.g., required fields)
	•	✅ API errors (e.g., duplicate user, wrong password)
	•	✅ Database via Prisma Studio

🎥 👉 Click here to watch the demo video

Ensure this link is public (anyone with link can view).


Made with 💻 by Mohd Aahil Uddin
As part of the IntelliSQR internship assignment.

---

### ✅ What You Should Do Now:

1. Copy this entire content into a file called `README.md` in the **root** of your repo.
2. Add `frontend/README.md` and `backend/README.md` (from earlier message).
3. Make sure `.env.example` files exist.
4. Push to GitHub one last time:
```bash
git add .
git commit -m "Add all README files and finalize project"
git push

