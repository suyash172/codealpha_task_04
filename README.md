Make sure you have the following installed:

Node.js (v18+ recommended)

npm or yarn

Git

Database (MongoDB / PostgreSQL / MySQL – as per project)

🔐 Environment Variables Setup
1️⃣ Backend .env setup

Go to the backend folder:

cd backend


Create a .env file:

touch .env


Add the required environment variables:

PORT=5000
DATABASE_URL=your_database_url
JWT_SECRET=your_jwt_secret
NODE_ENV=development


⚠️ Never commit .env files to GitHub.

2️⃣ Frontend .env setup

Go to the client folder:

cd client


Create a .env file:

touch .env


Example:

VITE_API_BASE_URL=http://localhost:5000/api


(Use REACT_APP_ prefix if using Create React App)

📦 Install Dependencies
Backend
cd backend
npm install

Frontend
cd client
npm install

▶️ Run the Project
Start Backend Server
cd backend
npm run dev


Backend will run on:

http://localhost:5000

Start Frontend Client
cd client
npm run dev


Frontend will run on:

http://localhost:5173


(or 3000, depending on setup)

🔁 Running Both (Optional)

If configured with concurrently:

npm run dev


This will start both client and backend together.

🧪 Scripts
Backend
npm run dev     # Start server in development
npm run start   # Start server in production

Frontend
npm run dev     # Start frontend
npm run build   # Build for production

🛠️ Tech Stack

Frontend: React / Next.js / Vite

Backend: Node.js, Express

Database: MongoDB / PostgreSQL

Auth: JWT

Containerization: Docker (optional)

📌 Notes

Make sure backend is running before frontend.

Check .env values carefully if API is not working.

Use correct API base URL in frontend.
