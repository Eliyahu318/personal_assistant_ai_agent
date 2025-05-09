﻿# persomal_asistant_ai_ajent
# 🤖 Personal AI Assistant

A smart personal assistant built with Python and OpenAI's GPT-4o, designed to understand Hebrew natural language commands.  
It manages tasks, stores and deletes them with confirmation, keeps chat history, and is ready for future integration with WhatsApp via Twilio or Render.

---

## ✨ Features

- 🧠 Natural language understanding (in Hebrew!)
- 📝 Add tasks with description and optional time
- ❌ Delete tasks intelligently (with GPT-based intent detection)
- 📚 Keeps full chat history between you and the assistant
- 🔄 Supports full reset of state
- 💾 File-based state persistence using JSON
- 🧪 Full test suite with `pytest`
- 📲 Future-ready for WhatsApp integration via Twilio or similar

---

## 📦 Project Structure

```
.
├── assistant.py          # Core logic and PersonalAssistant class
├── gpt_client.py         # Isolated OpenAI GPT communication
├── storege.py            # File management (JSON/JSONL logs)
├── prompts.py            # Prompt templates for GPT
├── whatsapp_server.py    # Placeholder for WhatsApp webhook server
├── data/                 # Persistent data (tasks, logs)
├── tests/                # Pytest test suite
├── main.py               # CLI entry point
└── .env                  # Environment variables (excluded from Git)
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/personal_ai_assistant.git
cd personal_ai_assistant
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Create `.env` file
```env
OPENAI_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxx
```

### 4. Run the assistant
```bash
python main.py
```

---

## 🧪 Run Tests

```bash
pytest tests/
```

---

## 🌐 Upcoming Integrations

- ✅ WhatsApp bot via Twilio
- ✅ Deployment on Render
- 🖥️ Web UI (Flask or FastAPI)
- 🗂️ Multi-user support

---

## ⚠️ Secrets & Security

Make sure `.env` is listed in `.gitignore` and **never commit your API key**. GitHub will block pushes containing secrets.

---

## 📝 License

MIT License

---

Built with 💙 by [Eliyahu](https://github.com/Eliyahu318)
