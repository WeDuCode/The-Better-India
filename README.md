🌐 The Better India – Advanced Search (Capstone Project)
An advanced search web application built using the MERN stack (MongoDB, Express, React, Node.js) that allows users to search through categorized articles, filter by tags, and narrow results by a date range. This project aims to improve user experience by offering intuitive filtering and seamless data presentation.

🔍 Features
🔤 Keyword-based text search

📂 Category selection (Events, Stories, Projects)

🏷️ Multi-tag filter (Education, Health, Innovation)

📆 Date range filtering (start and end date)

📄 Paginated and styled result display

⚡ Backend with Express + MongoDB (Mongoose)

🧠 Frontend with React, Axios, and CSS Modules

🛠️ Technologies Used
Frontend	Backend	Database	Tools
React	Node.js + Express	MongoDB	MongoDB Compass
Axios	CORS	Mongoose	Nodemon
React Router	dotenv		Postman (optional)

📁 Folder Structure
pgsql
Copy
Edit
the-better-india-search/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   │   ├── SearchPage.js
│   │   │   └── SearchPage.css
│   │   └── App.js
│   └── public/
├── package.json (both frontend and backend)
└── README.md
🚀 Getting Started
1️⃣ Backend Setup
bash
Copy
Edit
cd backend
npm install
Create .env file in /backend:

ini
Copy
Edit
PORT=5000
MONGO_URI=mongodb://localhost:27017/thebetterindia
Run backend server:

bash
Copy
Edit
npm run dev
2️⃣ Frontend Setup
bash
Copy
Edit
cd frontend
npm install
Start the React app:

bash
Copy
Edit
npm start
📦 Sample API Endpoint (Search)
http
Copy
Edit
GET http://localhost:5000/api/articles/search?search=green&category=Projects&tags=Innovation,Health&startDate=2024-01-01&endDate=2025-12-31
💡 How It Works
User enters a search keyword and optional filters (category, tags, date range).

React sends a request using Axios to the backend API.

Backend handles the request, builds a Mongoose query, and fetches matching results.

Results are sent back to frontend and displayed dynamically.

🖼️ Screenshots
💡 Include relevant screenshots of UI, search results, MongoDB Compass UI, etc.

🐞 Common Errors & Fixes
Error: Identifier 'useState' has already been declared

✅ Fix: Remove duplicate useState declaration or merge imports correctly.

Warning: 'useEffect' is defined but never used

✅ Fix: Either use useEffect or remove it from the import.

🧠 Future Enhancements
⏳ Add pagination with page controls

📥 Allow users to export results

🧼 Add a reset filter button

🔒 Add authentication layer (JWT)

📊 Visualize tag frequency or categories via charts