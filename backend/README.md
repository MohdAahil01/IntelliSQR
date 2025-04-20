##  `/backend/README.md`

```md
# IntelliSQR – Backend

This is the backend of the IntelliSQR full-stack authentication app, built using **Node.js**, **Express**, **TypeScript**, and **Prisma** ORM.

---

## ⚙️ Tech Stack

- Node.js + Express
- TypeScript
- Prisma ORM
- SQLite (or PostgreSQL)
- Bcrypt (for password hashing)
- JSON Web Tokens (for secure login, optional)
- CORS and error handling middleware

---

## 🛠️ Setup Instructions

### 1. Navigate to the backend folder

```bash
cd backend

### 2. Install dependencies

```bash
npm install

### 3. Configure environment variables
Create a .env file in the root of backend/:

```env 
DATABASE_URL="file:./dev.db"
JWT_SECRET=your_jwt_secret_here

### 4. Setup the database
Initialize Prisma and create the DB tables:

```bash
npx prisma migrate dev --name init

OR if you’ve already migrated once:
```bash
npx prisma db push

You can open a visual DB UI with:
```bash 
npx prisma studio

### 5. Start the backend server
npm run dev

Runs on: http://localhost:3005

## Folder Structure
backend/
├── src/
│   ├── controllers/      # Business logic for register/login
│   ├── routes/           # API endpoints
│   ├── middlewares/      # Error handler
│   ├── app.ts            # Express app setup
│   └── server.ts         # Server entry point
├── prisma/
│   ├── schema.prisma     # Database schema
├── .env.example
├── tsconfig.json
└── package.json

## API Endpoints

POST /api/users/register
	•	Registers a new user
	•	Body:  {
  "email": "user@example.com",
  "password": "securepassword"
}

POST /api/users/login
	•	Logs in a registered user
	•	Returns success or error message

## Features
	•	Fully working API for user registration and login
	•	Prisma-managed database with SQLite
	•	Hashed password storage using bcrypt
	•	Clean error handling and validation


