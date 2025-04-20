# IntelliSQR – Frontend

This is the frontend of the IntelliSQR full-stack authentication application built using **React**, **TypeScript**, and **Tailwind CSS**.

---

## 🚀 Tech Stack

- React + TypeScript
- Vite (frontend bundler)
- Tailwind CSS (styling)
- React Hook Form + Zod (form handling & validation)
- Axios (API requests)
- React Router DOM (routing)
- React Query (optional data fetching)

---

## 🛠️ Setup Instructions

### 1. Navigate to the frontend folder

```bash
cd frontend

### 2, Install dependencies
npm install

### 3. Configure environment variables

Create a .env file in the frontend root:

VITE_API_URL=http://localhost:3005/api

### 4. Start the development server
npm run dev

The frontend will run on: http://localhost:5173



## Folder Structure

 frontend/
├── src/
│   ├── pages/         # Login and Register pages
│   ├── lib/           # Zod schemas
│   ├── App.tsx        # Main routing file
│   └── main.tsx       # App entry point
├── public/
├── index.html
├── tailwind.config.js
└── .env.example

### Features
	•	Beautiful login/register UI styled with Tailwind
	•	Client-side validation using Zod
	•	Routing between pages using React Router
	•	Clear error handling and user feedback
