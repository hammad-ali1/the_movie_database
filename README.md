# the_movie_database
This repository is a clone of [TMDB](https://www.themoviedb.org) site. It uses the free TMDB api to fetch latest movies. The deployed site is at [this](https://tmdbv2.vercel.app) url. The site is deployed on vercel. The project was made using express with ejs for server side rendering. An admin panel is also deployed which was written using ReactJS. The project was an assignment for my university course on web technologies. 


## 📁 Project Structure

```
the_movie_database/
│
├── client/      # ReactJS-based admin panel
└── server/      # Express.js server with EJS rendering
```

---

## 🚀 Getting Started

Follow the steps below to set up and run both the client and server locally.

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/the_movie_database.git
cd the_movie_database
```

---

## 🔧 Server Setup (`/server`)

### Install Dependencies

```bash
cd server
npm install
```

### Create `.env` File

Inside the `server/` folder, create a `.env` file and add the following environment variables:

```
MONGO_URI=your_mongodb_connection_string
SESSION_SECRET=your_session_secret
PORT=5000
MOVIE_API_KEY=your_tmdb_api_key
```

You can get your `MOVIE_API_KEY` by creating a free account on [TMDB](https://www.themoviedb.org/documentation/api).

### Run the Server

```bash
npm start
```

---

## 🖥️ Client Setup (`/client`)

### Install Dependencies

```bash
cd client
npm install
```

### Run the Client

```bash
npm start
```

By default, the client runs on `http://localhost:3000`.

---

## 📌 Notes

- Make sure MongoDB is running locally or provide a valid remote URI in the `.env` file.
- The server must be running for the client (admin panel) to work properly if they communicate directly.
- The deployed version uses [Vercel](https://vercel.com) for the client. The backend should be deployed separately (e.g., on Render, Railway, or any Node.js-supporting host).
