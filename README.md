# Gemini AI Toolkit 🤖

A multi-feature AI-powered web application built using **HTML, CSS, JavaScript (Tailwind CSS)**, and the **Google Gemini API**. All features run from a single HTML file with one shared API key — no backend required.

---

## ✨ Features

| Tool | Description |
|------|-------------|
| 💬 **Simple Chatbot** | Have real-time conversations powered by Gemini |
| 🧠 **Prompt Practice** | Practice prompt engineering with modes: Summarize, Captions, Formal, Certificate, Compare |
| ❓ **Ask AI Anything** | Get concise 2–4 sentence answers to any question |
| 📝 **Summarizer** | Paste long text and get a beginner-friendly summary instantly |
| 🎭 **Tone Converter** | Rewrite text in Professional, Friendly, Formal, or Casual tone |
| 🖼️ **Caption Generator** | Generate Instagram, LinkedIn & General captions via structured JSON |
| 🏅 **Certificate Generator** | Auto-generate certificate text with a styled preview and copy option |
| 📄 **Resume Booster** | Paste weak resume bullets and get impact-focused rewrites |
| 🎨 **Theme Suggestions** | Describe a project and get a full UI color palette + font suggestions as JSON |

---

## 🛠️ Tech Stack

- **Frontend:** HTML, Tailwind CSS (CDN), Vanilla JavaScript
- **AI:** Google Gemini API (`gemini-3.5-flash`)
- **Storage:** LocalStorage (for API key management)
- **Concepts Used:** Prompt Engineering, Structured JSON responses (`application/json`), DOM Manipulation, Async/Await

---

## 🚀 Getting Started

### Prerequisites
- A valid [Google Gemini API Key](https://makersuite.google.com/app/apikey)
- A modern web browser (Chrome, Firefox, Edge)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kinjal-7166/Gemini-AI-Toolkit.git
   cd Gemini-AI-Toolkit
   ```

2. **Open the project**
   ```bash
   # Simply open project_ai.html in your browser
   open project_ai.html
   ```

3. **Enter your Gemini API Key**
   - Paste your Gemini API key in the input at the top of the page
   - Click **Save Key** — it gets stored in your browser's LocalStorage
   - All 9 tools will now work with this single key

---

## 📁 Project Structure

```
Gemini-AI-Toolkit/
│
├── project_ai.html     # Entire application (HTML + CSS + JS in one file)
└── README.md
```

---

## 🔑 API Key Management

Your Gemini API key is stored in **LocalStorage** and is only sent directly to Google's Gemini API. It is never shared or stored anywhere else.

To reset your key: Open browser DevTools → Application → LocalStorage → delete the `gemini_api_key` entry.

---

## 💡 How Prompt Engineering is Used

Each tool uses carefully crafted prompts to get reliable, structured responses:

- **Summarizer** — instructs the model to return beginner-friendly bullet summaries
- **Tone Converter** — specifies the target tone and constrains output to rewritten text only
- **Caption Generator** — uses `geminiJSON()` to return structured `{ instagram, linkedin, general }` captions
- **Certificate Generator** — returns structured JSON with recipient name, course title, duration, and blurb
- **Theme Suggestions** — returns a full palette, font, and background idea as structured JSON
- **Resume Booster** — prompts Gemini to act as a resume expert and return impact-focused rewrites

---

## 🙋‍♀️ About

Built as part of a **Deep Learning Internship at UptoSkills**, this project demonstrates how the Gemini API can be integrated into a lightweight single-file frontend to create practical, real-world AI tools — no backend, no framework, just clean JavaScript and smart prompts.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> ⭐ If you found this project helpful, consider giving it a star!
