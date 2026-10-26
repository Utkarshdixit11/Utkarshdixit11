<p align="center">
  <img src="screenshot/logo.svg" alt="SlaySheet Logo" width="72" height="72" />
</p>

<h1 align="center">SlaySheet</h1>

<p align="center">
  <strong>Write Together. Think Faster. Powered by Gemini AI.</strong><br>
  <em>A next-generation collaborative document workspace featuring live multiplayer editing, keystroke-level version time travel, an integrated Gemini AI writing partner, ambient focus soundscapes, and curated executive templates.</em>
</p>

<p align="center">
  🚀 <strong>Live Link:</strong> <a href="https://slay-sheet.vercel.app/" target="_blank"><strong>[SlaySheet]</strong></a> (https://slay-sheet.vercel.app/)
</p>

<p align="center">
  <a href="https://slay-sheet.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Live_Link-SlaySheet-10B981?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Link" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-19.2-61DAFB?logo=react&logoColor=black" alt="React 19" />
  <img src="https://img.shields.io/badge/Vite-8.1-646CFF?logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Node.js-18+-339933?logo=node.js&logoColor=white" alt="Node.js" />
  <img src="https://img.shields.io/badge/Express-5.2-000000?logo=express&logoColor=white" alt="Express" />
  <img src="https://img.shields.io/badge/Socket.IO-4.8-010101?logo=socket.io&logoColor=white" alt="Socket.IO" />
  <img src="https://img.shields.io/badge/Gemini_AI-2.1-4285F4?logo=google&logoColor=white" alt="Google Gemini" />
  <img src="https://img.shields.io/badge/MongoDB-9.8-47A248?logo=mongodb&logoColor=white" alt="MongoDB" />
</p>

---

## 📸 Key Features & Visual Showcase

### 1. Modern Landing Experience & Hero
A glassmorphic capsule navigation bar, iridescent 3D pearl aesthetics, and direct calls to action tailored for high-velocity teams.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20150013.png" alt="SlaySheet Landing Experience" width="100%" />
</p>

---

### 2. Collaborative Workspace Dashboard
Central command center for organizing your document library, tracking cloud storage, monitoring team collaborations, and launching quick actions.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20145824.png" alt="SlaySheet Dashboard" width="100%" />
</p>

---

### 3. Word Processor Canvas with "Live People" Presence
True-to-life standard Letter document pagination, rich typography studio (Google Fonts, custom sizing, headings, alignments), live word/character counts, and real-time live presence.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20145854.png" alt="Word Processor Canvas" width="100%" />
</p>

* **"Live People" Status**: Real-time room presence showing connected collaborators with active socket avatars, falling back cleanly to the document owner's profile when working solo.
* **Smart Page Breaks**: Automatically calculates Letter standard 96 DPI dimensions with seamless overflow.

---

### 4. Integrated Gemini AI Writing Partner
Context-aware AI sidecar assistant drawer accessible directly within your editor canvas.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20145902.png" alt="Gemini AI Writing Partner" width="100%" />
</p>

* **One-Click Actions**: Summarize document, improve clarity & tone, fix grammar & spelling, and brainstorm outlines.
* **Interactive AI Chat**: Conversational prompt assistance powered by Google Gemini.

---

### 5. Keystroke "Time Machine" (Version Replay & Audit Trail)
Replay the entire evolution of your document keystroke-by-keystroke with author attribution and one-click rollback.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20145939.png" alt="Keystroke Time Machine" width="100%" />
</p>

* **Granular Audit Trail**: Understand who wrote each sentence with exact timestamps.
* **Playback Controls**: Variable playback speed (`0.5x`, `1x`, `2x`, `5x`) and visual timeline scrubber.

---

### 6. Real-Time Multiplayer & Live Remote Cursors
Collaborate simultaneously with colleagues with fluid cursor broadcasting, live selections, and non-blocking sync.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20150023.png" alt="Multiplayer and Remote Cursors" width="100%" />
</p>

---

### 7. Curated Executive Starter Templates
Jumpstart new projects with structured starters accompanied by custom handwritten guidance.

<p align="center">
  <img src="screenshot/Screenshot%202026-09-12%20150107.png" alt="Starter Templates Showcase" width="100%" />
</p>

* **Product Requirements Document (PRD)**
* **Weekly Standup & Meeting Notes**
* **Client Project Proposal**
* **Engineering Sprint Plan**
* **Academic Research & Whitepaper**

---

## 🎧 Additional Innovation: Ambient "Zen Focus" Studio
Built directly into the editor status bar, SlaySheet features a procedural sound synthesizer generating **432Hz binaural alpha beats**, **rain on windowpane**, **library vinyl crackle**, and **gentle white noise** paired with an integrated Pomodoro timer.

---

## 🛠️ Architecture & Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend Framework** | [React 19](https://react.dev/), [Vite](https://vitejs.dev/) |
| **Rich Text Editor Engine** | [TipTap 3](https://tiptap.dev/) (`@tiptap/react`, `@tiptap/pm`, `@tiptap/starter-kit`) |
| **Styling & Design System** | TailwindCSS, Glassmorphism, Google Fonts (`Inter`, `Playfair Display`, `Fira Code`, etc.) |
| **Icons & Visuals** | [Lucide React](https://lucide.dev/) |
| **Real-Time Networking** | [Socket.IO](https://socket.io/) (client & server) with cursor tracking & presence room management |
| **Audio Engine** | Web Audio API procedural synthesis (`zenAudio.js` for binaural beats, noise, and vinyl crackle) |
| **Backend Runtime** | [Node.js](https://nodejs.org/), [Express 5](https://expressjs.com/) |
| **Database & ODM** | [MongoDB](https://www.mongodb.com/), [Mongoose 9](https://mongoosejs.com/) |
| **Artificial Intelligence** | [Google Gen AI SDK](https://github.com/google/generative-ai-js) (`@google/genai` with Gemini models) |
| **Authentication & Security**| JWT (JSON Web Tokens), `bcryptjs` password hashing |

---

## 🚀 Getting Started Locally

### Prerequisites
* **Node.js**: v18.0.0 or later
* **npm** or **yarn**
* **MongoDB**: Local MongoDB instance or MongoDB Atlas connection string
* **Gemini API Key**: From [Google AI Studio](https://aistudio.google.com/)

---

### 1. Clone the Repository
```bash
git clone https://github.com/Utkarshdixit11/SlaySheet.git
cd SlaySheet
```

---

### 2. Backend Setup
```bash
cd backend
npm install
```

Create a `.env` file in the `backend/` directory:
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/slaysheet
JWT_SECRET=your_super_secret_jwt_key
GEMINI_API_KEY=your_gemini_api_key_here
```

Start the backend server:
```bash
node server.js
# Backend runs on http://localhost:5000
```

---

### 3. Frontend Setup
In a new terminal window:
```bash
cd frontend
npm install
npm run dev
# Frontend runs on http://localhost:5173
```

Open `http://localhost:5173` in your browser to start writing and collaborating!

---

## 📂 Project Structure

```
SlaySheet/
├── backend/
│   ├── config/              # Database connection
│   ├── middleware/          # JWT authentication middleware
│   ├── models/              # Mongoose schemas (User, Document, Workspace, Revision)
│   ├── routes/              # Express API endpoints (auth, documents, ai, workspaces)
│   ├── server.js            # Express app & Socket.IO realtime server entry point
│   └── package.json
│
├── frontend/
│   ├── public/              # Static assets & favicon
│   ├── src/
│   │   ├── components/      # UI Views & Core Components
│   │   │   ├── AboutPage.jsx          # Interactive developer portfolio & matrix blast canvas
│   │   │   ├── Dashboard.jsx          # Documents hub & analytics
│   │   │   ├── DocumentEditor.jsx     # TipTap editor, live presence & typography studio
│   │   │   ├── LandingPage.jsx        # Showcase landing experience with capsule navbar
│   │   │   ├── Login.jsx & Register.jsx # Authentication views
│   │   │   ├── TimeMachineModal.jsx   # Keystroke version replay timeline
│   │   │   └── WorkspaceView.jsx      # Team workspaces & organization
│   │   ├── utils/
│   │   │   └── zenAudio.js            # Web Audio procedural sound generator
│   │   ├── App.jsx                    # Route definitions
│   │   ├── main.jsx                   # React root mount
│   │   └── index.css                  # Global styles & font bindings
│   ├── package.json
│   └── vite.config.js
│
├── screenshot/              # Curated showcase screenshots & logo
│   ├── logo.svg
│   └── ...
└── README.md                # Comprehensive documentation
```

---

## 👨‍💻 Author & Developer

Crafted with passion by **Utkarsh Dixit**.  
* **Education**: Bachelor of Computer Applications (BCA), SRMCM Lucknow (2024–2027)
* **Specialization**: Full-Stack Web Development, Real-Time Systems & AI Application Engineering

---

## 📄 License
This project is licensed under the [ISC License](LICENSE).  
© 2026 SlaySheet. All rights reserved.
