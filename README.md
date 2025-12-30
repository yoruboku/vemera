# Vemera | Infinite Streaming

<div align="center">
  <img src="https://via.placeholder.com/1200x500.png?text=Vemera+Preview" alt="Vemera Banner" width="100%" />
  <br/>
  <br/>
  <a href="https://github.com/yoruboku/vemera">
    <img src="https://img.shields.io/badge/Maintained%3F-yes-green.svg" alt="Maintained">
  </a>
  <a href="https://github.com/yoruboku/vemera">
    <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License">
  </a>
</div>

**Vemera** is a sleek, next-generation streaming frontend that aggregates movies, TV shows, and anime into a stunning, glassmorphic interface. Built with pure vanilla HTML, CSS, and JS, it requires no backend installation and runs entirely in the browser.

## ✨ Features

Vemera focuses on providing a **premium User Interface** experience often missing in open-source streaming sites.

* **🎨 Dynamic Design System:** A beautiful dark-mode interface with glassmorphism effects, smooth transitions, and responsive layouts that work on mobile and desktop.
* **🌈 Custom Theming:** Users can personalize the accent color of the entire site using a live hue slider in Settings.
* **💾 Local Profile System:** No signup required. Vemera uses LocalStorage to save your:
    * **Watch History** (Resume where you left off)
    * **Progress Tracking** (Visual progress bars on cards)
    * **Settings & Preferences**
* **⚡ Multi-Source Streaming:** Equipped with **12+ different streaming servers** to ensure maximum uptime and video quality. If one link fails, you can instantly switch to another via the player control bar.
* **🔍 Smart Search & Discovery:** Real-time search for Movies, TV Shows, and Anime, plus curated "Trending" and "Collection" lists.
* **🍿 Collections:** Browse by network (Netflix, HBO, Disney+, etc.) or movie franchises (Marvel, DC, etc.).

---

## ⚙️ Configuration (Required)

Before hosting, you must add your own API Key.

1.  Register for a free account at [The Movie Database (TMDb)](https://www.themoviedb.org/).
2.  Go to your account settings and generate an **API Key**.
3.  Open `index.html` in your code editor.
4.  Find **Line 407** (approx) inside the `<script>` tag:
    ```javascript
    // REPLACE THIS
    const API = "YOUR_TMDB_API_KEY_HERE";
    ```
5.  Paste your key inside the quotes.

---

## 🚀 How to Host

Since Vemera is a static web application (HTML/JS only), hosting it is incredibly easy and free.

### Option 1: GitHub Pages (Recommended)
1.  Fork this repository to your own GitHub account.
2.  Go to your repository **Settings**.
3.  Click on **Pages** in the left sidebar.
4.  Under **Source**, select `Deploy from a branch`.
5.  Under **Branch**, select `main` (or `master`) and `/ (root)`.
6.  Click **Save**. GitHub will generate a link (e.g., `yourname.github.io/vemera`) in a few minutes.

### Option 2: Netlify
1.  Log in to [Netlify](https://www.netlify.com/).
2.  Click **"Add new site"** -> **"Import from existing project"**.
3.  Connect to GitHub and select your Vemera repo.
4.  Click **Deploy Site**.
5.  *Alternatively:* You can simply drag and drop the folder containing `index.html` directly onto the Netlify dashboard to deploy manually.

### Option 3: Local Testing with Ngrok
If you want to test the site locally but share it with friends or test it on your phone:

1.  Download and install [Ngrok](https://ngrok.com/).
2.  Start a local server in your project folder.
    * *VS Code:* Use the "Live Server" extension.
    * *Python:* Run `python3 -m http.server 8000` in your terminal.
3.  Open a new terminal window and run ngrok pointing to your local port:
    ```bash
    ngrok http 8000
    ```
4.  Copy the `https://....ngrok-free.app` link provided in the terminal and share it.

---

## 🎮 Usage Guide

1.  **Login:** Enter any username to create a local profile. This is strictly local to your device; no password is sent to any server.
2.  **Player Controls:**
    * **Server Switcher:** Located at the top of the player. If a video buffers or doesn't load, use the dropdown to select a different source.
    * **Playlist:** Click the "List" button in the player to see other episodes or related movies.
3.  **Anime Support:** Anime is automatically detected. If a dub/sub is missing, try switching servers.

---

## 🤝 Credits

**Created & Maintained by [Yoruboku](https://github.com/yoruboku)**

If you enjoy this project, please consider starring the repository! 🌟
