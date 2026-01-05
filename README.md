# 📬 Smart Email Assistant (AI-Powered)

A **Smart Email Assistant** built with **Spring Boot + React (Material UI)** that generates intelligent email replies using **Google Gemini API**. The project also includes a **Chrome Extension** to provide email auto-suggestions directly inside the browser.

---

## 🚀 Features
* ✨ AI-powered email reply generation using **Google Gemini API**
* ⚙️ Backend built with **Spring Boot 3**
* 🎨 Modern frontend using **React + Material UI (MUI)**
* 🌐 REST API-based communication between frontend & backend
* 🧩 **Chrome Extension** for instant email suggestions
* 🧪 Tested with real email prompts
* 🔐 Secure API key handling via environment variables

---

## 🧑‍💻 Tech Stack

### Backend

* Java 17+
* Spring Boot 3
* Spring Web
* Google Gemini API

### Frontend
* React (Vite)
* Material UI (MUI)
* Axios

### Browser Extension

* Chrome Extension (Manifest v3)
* HTML, JavaScript
---

---

## 🔑 Environment Configuration

### Backend (`application.yml`)
```yml
gemini:
  api:
    key: YOUR_GEMINI_API_KEY
```

---

## ▶️ How to Run

### 1️⃣ Backend

```bash
cd backend
mvn spring-boot:run
```

Runs on: `http://localhost:8080`

---

### 2️⃣ Frontend (React + MUI)

```bash
cd frontend
npm install
npm run dev
```
Runs on: `http://localhost:5173`

---

### 3️⃣ Chrome Extension

1. Open Chrome → `chrome://extensions`
2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select `chrome-extension/` folder

---

## 🎨 UI (React + Material UI)

* Clean and responsive UI using **Material UI components**
* Email input using `TextField`
* Tone selector using `Select` & `MenuItem`
* Generate button with loading state (`CircularProgress`)
* Output displayed using `Typography` and `Box`

**User Flow:**
1. User enters email content
2. Selects reply tone (Professional, Friendly, Formal)
3. Clicks **Generate Reply**
4. AI-generated email response is displayed instantly

---

## 🧩 Chrome Extension Features
* Popup-based UI
* Calls Spring Boot API
* Auto-suggests email replies
* Can be integrated with Gmail-like workflows

---

## 🧪 API Endpoint Example
```
POST /api/email/generate
```

**Request Body:**

```json
{
  "emailContent": "Request for project deadline extension",
  "tone": "Professional"
}
```

## 📄 License

This project is for **learning and portfolio purposes**.

---

## 🙌 Acknowledgement
Inspired by AI-powered productivity tools using **Spring Boot + Gemini API**.

---

