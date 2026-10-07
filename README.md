# 🎬 CinePulse - Movie Explorer Application

> A modern, responsive React-based application built for searching, exploring, rating, and saving movies using The Movie Database (TMDB) public API.

---

## 🚀 Features & Requirement Alignment

| Requirement | Implementation Details | Status |
| :--- | :--- | :---: |
| **Search Movies** | Instant search bar with debounced input, live query filtering, and single-click clear functionality. | ✅ Completed |
| **View Movie Details** | Interactive modal displaying full backdrop, plot overview, release date, runtime, cast with portraits, similar movie recommendations, and YouTube trailer playback. | ✅ Completed |
| **Display Ratings** | Color-coded rating badges (Green >7.5, Yellow 6-7.5, Red <6), star breakdown, plus interactive personal 5-star user ratings saved in `localStorage`. | ✅ Completed |
| **Category Filters** | Interactive genre pills (Action, Comedy, Sci-Fi, Drama, etc.), minimum rating slider (All, 7+, 8+), and sort selector (Popularity, Top Rated, Release Date, Title). | ✅ Completed |
| **Responsive Design** | Cinematic dark design system built with Tailwind CSS v4, dynamic glassmorphism, responsive grid layout, and touch-friendly mobile navigation. | ✅ Completed |
| **Error Handling** | Graceful error states with diagnostic card, fallback offline movie dataset, and one-click retry / custom API key modal. | ✅ Completed |
| **Loading Indicators** | Shimmer skeleton loaders for grid cards and smooth loading states during API transitions. | ✅ Completed |

---

## 🛠️ Technology Stack & Skills Practiced

- **Frontend Framework**: React 19 + Vite 8
- **Styling & Aesthetics**: Tailwind CSS v4 + Vanilla CSS glassmorphism & micro-animations
- **Icons**: Lucide React
- **State Management**: React Context API (`MovieContext`) with custom hooks (`useMovieContext`)
- **API Integration**: TMDB REST API v3 with robust fallback dataset engine
- **Persistence**: `localStorage` sync for Watchlist and personal movie reviews/ratings

---

## 📂 Project Architecture

```text
c:\Users\venka\Downloads\varsha project\
├── public/
├── src/
│   ├── components/
│   │   ├── Navbar.jsx          # Brand header, tab navigation, search input & theme toggle
│   │   ├── HeroBanner.jsx      # Auto-rotating featured movie carousel with trailer trigger
│   │   ├── GenreFilters.jsx    # Genre pill badges, minimum rating filter, and sorting dropdown
│   │   ├── MovieCard.jsx       # Poster card with dynamic rating badge & hover overlay
│   │   ├── MovieGrid.jsx       # Main grid container, title header, skeletons & pagination
│   │   ├── MovieModal.jsx      # Detailed modal with cast, trailer, recommendations & user rating
│   │   ├── TrailerModal.jsx    # Embedded YouTube trailer video player
│   │   ├── WatchlistView.jsx   # Dedicated view for bookmarked movies & personal notes
│   │   ├── RatingComponent.jsx # Interactive 1-5 star rating & review note widget
│   │   ├── SkeletonCard.jsx    # Shimmer placeholder card
│   │   ├── ErrorState.jsx      # Fallback error container with retry action
│   │   └── SettingsModal.jsx   # TMDB API Key custom setup modal
│   ├── context/
│   │   └── MovieContext.jsx    # Application state management provider
│   ├── services/
│   │   ├── tmdbApi.js          # TMDB endpoints & network fallback handler
│   │   └── mockMovies.js       # Offline backup movie dataset
│   ├── App.jsx                 # Core layout assembly
│   ├── index.css               # Tailwind v4 directives & glass design tokens
│   └── main.jsx                # React root renderer
├── package.json
└── vite.config.js
```

---

## ⚙️ Local Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone <your-repository-url>
   cd varsha-project
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start local development server**:
   ```bash
   npm run dev
   ```
   Open your browser at `http://localhost:5173`.

4. **Build for Production**:
   ```bash
   npm run build
   ```

---

## 🌐 Deployment Instructions

### Option 1: GitHub Pages (Automated)
1. Add your GitHub repository as remote:
   ```bash
   git remote add origin https://github.com/<your-username>/movie-explorer-app.git
   git branch -M main
   git push -u origin main
   ```
2. Deploy to GitHub Pages:
   ```bash
   npm run deploy
   ```

### Option 2: Vercel / Netlify
1. Connect your GitHub repository directly to Vercel or Netlify.
2. Build command: `npm run build`
3. Output directory: `dist`

---

## 📄 License
This project is completed as a Movie Explorer Application assignment.
