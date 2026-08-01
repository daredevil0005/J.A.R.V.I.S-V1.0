# 🤖 J.A.R.V.I.S AI Voice Assistant

> 🚀 Real-time AI assistant with automation, memory, and system control

![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-15-000000?style=for-the-badge&logo=next.js)
![Node.js](https://img.shields.io/badge/Node.js-22+-339933?style=for-the-badge&logo=node.js&logoColor=white)
![LiveKit](https://img.shields.io/badge/LiveKit-Realtime-7C3AED?style=for-the-badge)
![Gemini](https://img.shields.io/badge/Google-Gemini_AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Windows](https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/daredevil0005/J.A.R.V.I.S-V1.0?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/daredevil0005/J.A.R.V.I.S-V1.0?style=for-the-badge)
![Issues](https://img.shields.io/github/issues/daredevil0005/J.A.R.V.I.S-V1.0?style=for-the-badge)
![Last Commit](https://img.shields.io/github/last-commit/daredevil0005/J.A.R.V.I.S-V1.0?style=for-the-badge)
![AI Assistant](https://img.shields.io/badge/Project-AI%20Voice%20Assistant-8A2BE2?style=for-the-badge)

---

## 🎯 Overview

J.A.R.V.I.S (Just A Rather Very Intelligent System) is a **real-time AI-powered voice assistant** that combines **Conversational AI + System Automation**.

It allows users to interact using voice commands and perform tasks like:

* Opening applications
* Searching the web
* Controlling system settings
* Managing media playback
* Storing and recalling memory

Built using **LiveKit + Google Realtime AI**, this project demonstrates practical implementation of modern AI systems.

---

## 🚀 Features

* 🎤 Real-time voice interaction
* 🧠 AI-powered responses (Google Realtime Model)
* ⚙️ System automation (open apps, WiFi, brightness, etc.)
* 🌐 Google search with voice summary
* 🖼️ Image search support
* 🧾 Memory storage & recall
* 🔊 Voice response output
* 🌍 LiveKit-based web UI

---

## 🧠 What Makes This Project Special

* ⚡ Real-time streaming using LiveKit
* 🤖 AI + Automation combined in one system
* 🎵 Smart media control:
  * YouTube (Play, Pause, Next, Previous)
  * VLC Media Player
  * System media (Spotify, etc.)
* 🧾 Memory system for personalized interaction
* 🌐 Full-stack architecture (Python + Node.js frontend)

---

## 🏗️ System Architecture

User → LiveKit UI → Assistant Core → AI Model → Tool Modules → Operating System

---

## 🛠️ Technologies Used

* Python
* LiveKit (Realtime Communication)
* Google Realtime AI (Gemini)
* Node.js
* WebRTC
* JavaScript

---

## 📸 Demo

### 🖥️ Home Screen
<p align="left">
  <img src="assets/1.png" width="70%" />
</p>

### 🎤 Voice Interaction
<p align="left">
  <img src="assets/2.png" width="70%" />
</p>

### 🎤 Text Interaction
<p align="left">
  <img src="assets/3.png" width="70%" />
</p>

---

## 📋 Prerequisites

Before installing and running **J.A.R.V.I.S**, make sure the following software is installed on your system:

| Software | Version | Purpose |
|----------|---------|---------|
| Python | 3.11+ | Runs the backend AI assistant |
| Node.js | 20+ | Required for the Next.js frontend |
| npm | Latest | Installs frontend dependencies (included with Node.js) |
| pnpm *(Optional)* | Latest | Alternative package manager for the frontend |
| Git *(Optional)* | Latest | Clone the repository and manage source code |

> **Note:** J.A.R.V.I.S supports both **npm** and **pnpm**. Use only one package manager for a given installation. If you switch package managers, delete the `node_modules` folder and reinstall the dependencies.

---

### Verify Installation

* python --version
* node -v
* npm -v

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository Or Download Zip File

* git clone https://github.com/daredevil0005/J.A.R.V.I.S-v1.0.git
* cd J.A.R.V.I.S-v1.0

---

### 2️⃣ Backend Setup (Python)

* py -m venv .venv - (Virtual enviroment setup)
* .\venv\Scripts\activate - (Activating Virtual enviroment)
* python -m pip install -r requirements.txt - (Installing required packages)

---

### 3️⃣ Environment Variables

* Create `.env` file in root folder:

* GOOGLE_API_KEY=your_api_key, 
* GOOGLE_SEARCH_API_KEY=your_search_key, 
* SEARCH_ENGINE_ID=your_engine_id, 
* LIVEKIT_URL=your_livekit_url, 
* LIVEKIT_API_KEY=your_livekit_key, 
* LIVEKIT_API_SECRET=your_livekit_secret, 

---

### 4️⃣ Run Backend To Test 

* python agent.py console

---

### 5️⃣ Frontend Setup
## Option 1 (Recommended - npm)

* cd agent-ui
* npm install
* npm run dev

## Option 2 (Alternative - pnpm)

* cd agent-ui
* npm install -g pnpm
* pnpm install 
* pnpm run dev

---

### 6️⃣ Open Application

* http://localhost:3000

---

## ⚠️ Important Notes

* Run backend and frontend in **separate terminals**
* Ensure `.env` file is properly configured
* Internet connection is required
* Microphone permission must be enabled

---

## 🧠 How It Works

1. User gives voice command
2. LiveKit captures and streams audio
3. AI processes input
4. Assistant decides:
   * Response → AI reply
   * Action → Tool execution
5. System performs action
6. Jarvis responds via voice

---

## ⚙️ Feature Workflow Example

### Example: “Open Chrome”

* 🎤 Input → Voice command
* 🧠 Processing → Intent detection
* ⚙️ Execution → Tool function call
* ✅ Output → Chrome opens + voice confirmation

---

## 🧾 Memory System

Jarvis can store and recall user data.
Jarvis uses a local SQLite database (memory.db) to store user memories and conversation history.

Example:

* “Remember my name is Pratik”
* “What is my name?”

✔ Stored in memory module
✔ Retrieved dynamically

---

## 🔍 Google Search Feature

* Uses search API
* Opens browser automatically
* Provides voice summary

---

## 🖼️ Image Search

* Opens Google Images
* Displays visual results

---

## 🧩 Project Structure

```
J.A.R.V.I.S/
│
├── agent.py
├── features/
├── memory/
├── agent-ui/
├── requirements.txt
└── .env
```

---

## 🔐 Security

* API keys stored in `.env`
* No hardcoded secrets
* Controlled system access via tools

---

## 🧪 Testing

Tested for:

* Voice input/output
* AI response generation
* System commands
* Memory storage
* Performance

---

## 🚀 Future Scope

* Wake word detection (“Hey Jarvis”)
* Cloud deployment
* Mobile app
* Multi-user support
* Smart home integration

---

## 👨‍💻 Author

**Pratik S. Dabhane**

---

## 🎯 Conclusion

J.A.R.V.I.S demonstrates **real-time AI interaction + automation + system control** in a single integrated system.

It showcases how modern AI technologies can be applied to build intelligent, interactive applications.

---

⭐ If you like this project, consider giving it a star!
