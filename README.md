Movie App

This is a Movie App built using React and Vite.
It allows users to browse, search, and view movie details — including titles, descriptions, ratings, and more.
This README provides setup instructions, project structure, environment configuration, and guidelines for production deployment.

Features
Display a list of movies
View detailed movie information
Search functionality
Filter and sort (by genre, rating, year)
Add/remove from favorites or watchlist
Responsive design (mobile & desktop)

Optional: Pagination, lazy-loading, client-side routing
 Tech Stack
React (functional components + hooks)
Vite (fast build tool)
React Router (navigation)
 Fetch API (data fetching)
Tailwind CSS / CSS Modules / Styled Components (styling)

Prerequisites
Make sure you have installed:
Node.js (v16 or higher)


 Installation & Local Setup
Clone the repository
git clone https://github.com/your-username/movie-app.git
cd movie-app


Install dependencies

npm install
# or
yarn install


Set up environment variables


Run the development server
npm run dev


Open your browser at http://localhost:5173


After building, the /dist folder contains optimized static files you can deploy to any hosting provider (Vercel, Netlify, GitHub Pages
 Environment Variables
Create a .env file in your project root (Vite requires variables to start with VITE_):
VITE_API_BASE_URL=https://api.themoviedb.org/3
VITE_API_KEY=your_tmdb_api_key_here
VITE_IMAGE_BASE_URL=https://image.tmdb.org/t/p/w500


 Never commit .env files containing API keys to public repositories.
Instead, include a .env.example file with placeholder values.

 Project Structure 
movie-app/
├─ public/
├─ src/
│  ├─ assets/
│  ├─ components/
│  │  ├─ MovieCard/
│  │  ├─ SearchBar/
│  ├─ pages/
│  │  ├─ Home/
│  │  ├─ MovieDetail/
│  ├─ hooks/
│  ├─ services/
│  │  ├─ api.js
│  ├─ context/
│  ├─ routes/
│  ├─ styles/
│  ├─ App.jsx
│  └─ main.jsx
├─ .env.example
├─ package.json
├─ vite.config.js
└─ README.md