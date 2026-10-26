# ⚔️ GridWars — Real-Time Territory Battle

![Node.js](https://img.shields.io/badge/Node.js-18-green)
![MongoDB](https://img.shields.io/badge/Database-MongoDB-brightgreen)
![WebSockets](https://img.shields.io/badge/Realtime-WebSockets-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

### 🌐 Live Deployment
Play the game live here: **[GridWars Live Arena](https://gridwars-7w1b.onrender.com/)**

---

## 📖 What is GridWars?

GridWars is a real-time, browser-based multiplayer territory conquest game. After registering a persistent user profile and choosing a unique color, players battle against other active warriors on a shared, dynamic grid to claim tiles. The objective is to claim territory, build adjacent combo streaks, and defend your tiles from being stolen in order to climb the leaderboard.

---

## 📁 Project Structure

Here is a quick overview of the file structure to help navigate the project:

```
GridWars/
├── backend/
│   ├── mongodb_data/       # Integrated local database directory
│   ├── models/             # Mongoose database models
│   └── server.js           # Express and WebSocket server
├── frontend/
│   ├── index.html          # Game HTML layout
│   ├── style.css           # UI Styling (glassmorphism/transitions)
│   └── app.js              # Client WebSocket and UI event logic
├── capture/                # Screenshots and visuals
├── .env                    # Active environment settings (git ignored)
├── .env.example            # Environment configuration template
├── start.js                # Smart local DB and server launcher
└── README.md               # Project documentation
```

---

##  Screenshots & Visuals

Here is a visual overview of GridWars in action, captured from the application:

### 1. Entrance Portal (Login & Registration)
We feature an immersive login screen with a widescreen panning animation transition upon entry:

![Login Screen](./capture/login.png)
*Figure 1: Clean, minimalist Login portal.*

![Registration Screen](./capture/signup.png)
*Figure 2: Account creation with dynamic color-palette selector.*

---

### 2. Main Arena & Gameplay
The main battlefield displays the grid, left navigation bar, live leaderboard standings, and bottom-right minimap:

![Battlefield Overview](./capture/Gridwar.png)
*Figure 3: Interactive GridWars battlefield.*

---

### 3. Dynamic Sidebar Navigation
Manage your avatar, view full leaderboard statistics, and configure setting profiles dynamically:

![Leaderboard Tab](./capture/leaderboard.png)
*Figure 4: Global Leaderboard panel.*

![Settings Tab](./capture/settings.png)
*Figure 5: In-game user profile settings.*

---

### 4. Administrative Controls
Specialized admin accounts (like `Gridadminutkarsh`) have access to a vertical management widget below the online indicator to control grid presets and reset matches:

![Admin Control Panel](./capture/admin_control.png)
*Figure 6: Admin floating panel (Reset Grid and Size options).*

---

## 🎮 Game Rules & Mechanics

### 1. Tile Capture
* Click any empty or unlocked cell on the grid to claim it. 
* Claimed tiles instantly assume your unique color and display your username's initial.
* Once captured, a tile remains **locked for 20 seconds**, preventing other players from stealing it. Once the lock expires, it can be reclaimed by opponents.

### 2. Cooldown
* After claiming a tile, a red sweeping timer border surrounds the tile indicating the cooldown duration (2.5 seconds).
* Click interactions are locked during cooldown to prevent spam-clicking.

### 3. Score Calculations & Combos
* **Base Capture**: Claiming an isolated tile awards **`10 points`**.
* **Adjacent Capture**: Claiming a tile that directly touches the boundary of one of your previously owned tiles awards **`15 points`** instead of 10.
* **🔥 Adjacent Combo Streak**: Capturing contiguous tiles forms a cluster. Directly above your newly claimed cell, a burst fire indicator shows your total cluster size (e.g. `🔥 3`).

---

## 🛠️ Technical Stack

GridWars is structured to be robust, secure, and ready for production:

* **Frontend**:
  * **Core**: Semantic HTML5, Vanilla ES6+ JavaScript.
  * **Design & Animations**: Pure CSS3 variables with sleek glassmorphism, responsive media layouts, and GPU-accelerated transition states.
  * **Canvas Render**: Dynamic canvas-driven minimap displaying a real-time scaled layout of the entire grid.
* **Backend**:
  * **Server**: Node.js & Express.
  * **Real-time Sync**: Standard WebSockets (`ws` library) for millisecond-latency events.
* **Database**:
  * **MongoDB**: Managed through **Mongoose ODM**. Saves persistent states for:
    * Users (credentials, leaderboard scores, and administrative privileges).
    * Grid Cells (active board cell locations, owners, colors, and lock timestamps).

---

## ⚙️ Environment Configuration

GridWars expects a `.env` file in the root directory. You can use the provided `.env.example` as a template:

```ini
# MongoDB Connection String (Atlas or Local URL)
MONGODB_URI=mongodb://127.0.0.1:27017/gridwars

# Port for the Node.js Express server to listen on
PORT=3000
```

---

## ⚡ Setup & Launch Instructions

### Prerequisites
* [Node.js](https://nodejs.org/) installed on your machine.
* MongoDB installed locally (defaults to standard `C:\Program Files\MongoDB\Server\...`).

### Installation
Clone the repository and install all dependencies:
```bash
npm install
```

### Running the Application
GridWars uses an integrated, single-command startup script. You do not need to run your MongoDB service separately:
```bash
npm start
```

* **What it does**:
  1. Locates your Windows MongoDB engine.
  2. Spawns a database instance pointing directly inside [backend/mongodb_data](./backend/mongodb_data).
  3. Boots up the Node server on `http://localhost:3000`.
  
Open `http://localhost:3000` in your browser and enter the arena!

---

## 📄 License & Contributing

MIT License — feel free to fork, open pull requests, and contribute to GridWars!

---

## 👤 Author

* **Utkarsh Dixit** — *Creator & Developer*
* LinkedIn: [linkedin.com/in/utkarshdixit9](https://www.linkedin.com/in/utkarshdixit9)
