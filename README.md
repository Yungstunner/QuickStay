QuickStay 🏕️
A platform to explore and book serene lakefront stays in a breeze.

🔗 Live Demo
quickstay-lake.vercel.app

🚀 Features
Browse curated lakeside properties.

Filter by price, location, and amenities.

Seamless user experience with responsive design.

Secure booking flow with form validation.

🧭 Tech Stack
Client: React (Vite) • React Router • Tailwind CSS

Server: Node.js • Express • MongoDB (Mongoose)

Authentication: JSON Web Tokens (JWT)

Deployment: Vercel (frontend) & Render/Heroku (backend)

📁 Project Structure
php
Copy
Edit
root/
├─ client/           # Frontend React application
│   ├─ public/       # Static assets
│   └─ src/          # Components, pages, hooks, services
│
├─ server/           # Backend API
│   ├─ controllers/  # Route handlers
│   ├─ models/       # Mongoose schemas
│   ├─ routes/       # API endpoints
│   └─ middleware/   # Auth and error handlers
│
├─ .gitignore
├─ README.md
└─ package.json      # For backend; client has its own
🛠️ Installation & Setup
Clone

bash
Copy
Edit
git clone https://github.com/Yungstunner/QuickStay.git
cd QuickStay
Install dependencies

bash
Copy
Edit
cd server
npm install

cd ../client
npm install
Environment variables

In server/.env:

ini
Copy
Edit
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
Run Development Servers

bash
Copy
Edit
# Server
cd server
npm run dev

# Client
cd ../client
npm run dev
Visit the frontend at http://localhost:5173 (or whichever port Vite picks).

🧪 API Endpoints
POST /auth/register – Sign up

POST /auth/login – Log in (returns JWT)

GET /properties – List stays (query filters supported)

GET /properties/:id – Property details

POST /bookings – Create booking (requires JWT)

📦 See server/routes for full specs and request/response formats.

✅ Contributing
Thanks for your interest!

Fork the repo

Create a feature branch: git checkout -b feature/your-feature

Commit your changes: git commit -m "Add awesome feature"

Push branch: git push origin feature/your-feature

Open a Pull Request

