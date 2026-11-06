# Jarvis-mark-1

# 🤖 MARK LVI (Jarvis)

**MARK LVI** is a high-performance, AI-driven personal assistant designed to act as a central operating system for your digital life. Combining the power of **Google Gemini Live** with deep system integration, MARK LVI doesn't just talk—it acts.

From controlling your browser and managing files to monitoring your system and rendering a holographic avatar, MARK LVI brings the "Jarvis" experience to your desktop.

---

## ✨ Key Features

### 🧠 Intelligence & Interaction
- **Gemini Live Integration**: Powered by the latest Google GenAI for fluid, natural conversations.
- **Holographic Avatar**: A software-rendered 3D head that reacts and poses in real-time without requiring a GPU.
- **Voice-to-Voice**: Integrated STT (Speech-to-Text) and TTS (Text-to-Speech) for a completely hands-free experience.
- **Wake Word Support**: Opt-in "Hey Jarvis" activation via `openwakeword`.

### 🛠️ System Automation (The "Actions" Engine)
MARK LVI can interact directly with your Windows OS:
- **Computer Control**: Adjust system settings, volume, and brightness.
- **File Management**: Process PDFs, Docx, and PPTX files; organize folders and manage trash.
- **Web Automation**: Full browser control via Playwright for searching, scraping, and navigating the web.
- **App Integration**: Open applications, manage game updates, and monitor system hardware (CPU/GPU/RAM).

### 📱 Remote Control
- **Web Dashboard**: A built-in FastAPI server that allows you to monitor and control your assistant from a smartphone or tablet via a secure web interface.

---

## 🚀 Quick Start

### Prerequisites
- **Python 3.12+**
- **Google AI Studio API Key** (for Gemini)

### ⚡ One-Click Installation (Windows PowerShell)
Copy and paste this single command into your terminal to clone, install, and run everything:

```powershell
git clone https://github.com/swastik20130201/Jarvis-mark-1.git; cd Jarvis-mark-1; python -m venv venv; .\venv\Scripts\activate; pip install -r requirements.txt; playwright install; python main.py

---

⚙️ Configuration

Once launched, navigate to ⚙ → ENGINE & PROVIDERS to:
1. Enter your Gemini API Key.
2. Choose your preferred TTS voice (System, Piper, or ElevenLabs).
3. Configure your STT provider (Whisper or Google).

---

📦 Architecture

- /core: The brain of the system (Audio, LLM Client, Action Loader).
- /actions: Modular scripts that allow the AI to perform specific tasks on your PC.
- /providers: Pluggable modules for different AI engines (OpenAI, Gemini, etc.).
- /dashboard: The FastAPI backend for the remote web interface.
- /memory: Long-term memory management for personalized interaction.

---

🤝 Contributing

Feel free to add new capabilities by dropping a new .py file into the /plugins folder. Follow the _template.py guide to ensure your plugin is loaded correctly.

License: MIT
