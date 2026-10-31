# AI Chat Assistant — High-Performance Streaming & Multi-Model Engine 🤖

[![Live Hosted](https://img.shields.io/badge/Live_Hosted-GitHub_Pages-22c55e?style=for-the-badge&logo=github)](https://meetaj369.github.io/AI-Chat-Assistant/)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Python 3.12](https://img.shields.io/badge/Python-3.12-3776ab?style=for-the-badge&logo=python&logoColor=white)](https://python.org/)
[![Claude 3.5](https://img.shields.io/badge/Claude_3.5-Anthropic-d97706?style=for-the-badge&logo=anthropic)](https://anthropic.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

An intelligent conversational web application and asynchronous backend engine featuring real-time Server-Sent Events (SSE) token streaming, multi-model routing (Claude 3.5 Sonnet, Gemini 1.5 Pro, GPT-4o), markdown syntax highlighting with one-click code copy, voice dictation, session memory persistence, and transcript export.

**Live Application**: [https://meetaj369.github.io/AI-Chat-Assistant/](https://meetaj369.github.io/AI-Chat-Assistant/)  
**Developer**: [Meet Chauhan](https://meetaj369.github.io/Meet-Portfolio/)

---

## ⚡ Core Capabilities

1. **Real-Time Token Streaming**: Continuous client-side streaming cadence via Server-Sent Events (SSE) / asynchronous generators with live typing cursor.
2. **Multi-Model Routing**: Seamlessly switch between Claude 3.5 Sonnet (coding/logic), Gemini 1.5 Pro (reasoning), GPT-4o (creative), and Meet's Portfolio Assistant.
3. **Markdown Syntax Parser**: Live parsing of fenced code blocks with language indicators, one-click copy buttons, bold/italic tokens, lists, and tables.
4. **Session Management**: Persistent multi-chat history saved to local storage with session renaming, searching, and deletion.
5. **Speech Dictation & Audio**: Voice input via Web Speech Recognition API and text-to-speech audio reader.
6. **Transcript Export**: Export any conversation session into formatted Markdown (`.md`) with timestamps and model metadata.

---

## 📁 System Architecture

```
AI-Chat-Assistant/
├── index.html              # Standalone liquid glass conversational application
├── assets/
│   ├── css/                # Custom stylesheets & syntax themes
│   ├── js/                 # Client state & speech recognition engines
│   └── img/                # Favicon and brand assets
├── backend/
│   ├── main.py             # FastAPI SSE streaming microservice
│   ├── requirements.txt    # Python dependencies
│   └── .env.example        # Environment variable configuration
├── api/
│   └── chat.php            # PHP SSE streaming proxy for Apache/WAMP
├── README.md               # Production documentation
└── LICENSE                 # MIT License
```

---

## 🚀 Quick Start Guide

### Frontend (Static Browser / GitHub Pages)
Open `index.html` directly in any modern browser or host via GitHub Pages, Vercel, or Netlify.

### Backend (Python FastAPI)
```bash
cd backend
python -m venv venv
venv\Scripts\activate      # Windows
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

### Local WAMP Server
Copy the `AI-Chat-Assistant` folder to `C:\wamp\www\` and access via `http://localhost/AI-Chat-Assistant/`.

---

## 📄 License
This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.  
Copyright (c) 2026 Meet Chauhan.
