# MindVoice — AI Voice Journaling for Emotional Well-being

## 📌 Overview
MindVoice is an AI-powered journaling application designed to help users monitor and understand their emotional well-being over time. The system enables users to record or write daily reflections, which are analyzed using Google Gemini AI to detect emotional tone, generate insights, and visualize mood trends.

The current prototype is implemented as a **web-based application with text input**, while the system architecture is designed to support **voice-first journaling using Speech-to-Text** in future iterations.

---

## 🎯 Problem Statement
Many individuals struggle to consistently monitor their mental health. Emotional patterns often go unnoticed until burnout, anxiety, or severe stress occurs. Traditional journaling lacks structured emotional analysis and long-term trend visualization.

MindVoice aims to provide **accessible, AI-assisted emotional awareness** to help users better understand and manage their mental well-being.

---

## 🌍 SDG Alignment
**SDG 3 — Good Health & Well-being**

MindVoice promotes early emotional awareness, self-reflection, and proactive mental health monitoring, supporting overall psychological well-being.

---

## 🤖 AI Integration (Google Gemini)
Google Gemini is used as the core AI engine to:

- Analyze emotional tone of journal entries
- Generate structured sentiment score (-1 to +1)
- Detect dominant emotional state (e.g., calm, stressed, anxious, positive)
- Produce concise AI-generated emotional summaries
- Enable future weekly emotional trend insights

AI is used meaningfully to transform unstructured personal reflections into actionable emotional insights.

---

## ☁️ Google Technologies Used
- **Google Gemini API** — Emotional analysis and AI insight generation  
- **Google Cloud Platform (GCP)** — Backend service infrastructure  
- **Firebase Hosting** — Web application hosting  
- **Cloud Firestore (planned / optional)** — Secure journal data storage  
- **Cloud KMS (planned / optional)** — Encryption for sensitive personal data  
- **Speech-to-Text (future integration)** — Voice journaling support  

---

## 🏗 System Architecture
1. User submits journal entry (current prototype: text-based; voice-ready architecture)
2. Backend server sends entry to Google Gemini API
3. Gemini analyzes emotional tone and generates sentiment + summary
4. Results returned to backend
5. Journal data stored securely (Firestore optional)
6. Frontend visualizes emotional trend and insights

---

## 🚀 How to Run the Project

### Prerequisites
- Java JDK 17+
- Node.js (if frontend uses JS)
- Google Cloud account with Gemini API enabled
- API Key configured

### Steps
1. Clone the repository  
   ```bash
   git clone https://github.com/your-repo/mindvoice.git
