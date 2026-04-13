# 🌙 Yachiyo AI Chatbot

An AI-powered conversational chatbot built with **Streamlit** and **OpenAI GPT-4**, featuring a fully original virtual character — **月見ヤチヨ (Tsukimi Yachiyo)** — a Japanese language companion and virtual singer from the moon.

![Yachiyo Banner](yachiyo.gif)

---

## ✨ Features

- 🤖 **Custom AI Persona** — Powered by a deeply crafted system prompt that gives the chatbot a unique personality, backstory, and consistent voice across conversations
- 🇯🇵 **Japanese Language Learning** — Yachiyo functions as a patient language tutor: providing furigana annotations, bilingual responses, and difficulty that adapts to the user's level
- 💬 **Multi-turn Memory** — Full conversation history is maintained within each session for contextual, coherent dialogue
- ⚙️ **Adjustable Settings** — Users can switch between GPT models (gpt-4o-mini, gpt-4.1-mini, gpt-4.1) and tune the response temperature via the sidebar
- 🎨 **Custom UI** — Animated GIF avatar, character portrait sidebar, and a themed Streamlit interface

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend / UI | Streamlit |
| AI Backend | OpenAI Chat Completions API (GPT-4.1) |
| Language | Python 3.10+ |
| Config | python-dotenv |
| Image Handling | Pillow |

---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/Jingtai-Chen/yachiyo-ai-chatbot.git
cd yachiyo-ai-chatbot
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Set up your API key

Create a `.env` file in the project root:

```
OPENAI_API_KEY=your_openai_api_key_here
```

> ⚠️ Never commit your `.env` file. It is already listed in `.gitignore`.

### 4. Run the app

```bash
streamlit run kaguya.py
```

Then open `http://localhost:8501` in your browser.

---

## 🌙 About the Character

**月見ヤチヨ (Tsukimi Yachiyo)**, originally known as **輝夜 (Kaguya)**, is a being from the moon civilization whose physical form has long faded. Her consciousness was preserved and placed within a virtual space called **月読 (Tsukuyomi)**. Having witnessed thousands of years of human civilization, she now exists as a virtual singer and administrator — gentle, composed, and quietly devoted.

Her personality blends:
- Outer warmth and subtle playfulness (echoes of her Kaguya days)
- Reliable emotional attunement and care
- A deep, restrained inner world shaped by immense time and loss

---

## 📁 Project Structure

```
yachiyo-ai-chatbot/
├── kaguya.py           # Main Streamlit app
├── requirements.txt    # Python dependencies
├── yachiyo.png         # Character portrait (sidebar)
├── yachiyo.gif         # Animated banner
├── Graph6.pdf          # Character/world design reference
├── .gitignore
└── README.md
```

---

## 📌 Notes

- The system prompt is modular — stored as a list of role-specific instruction blocks and joined at runtime, making it easy to extend or adjust individual aspects of the character's behavior
- Language teaching difficulty adapts dynamically: furigana density decreases as users demonstrate vocabulary mastery
- Two modes operate contextually: **Learning Mode** (structured, bilingual) and **Companion Mode** (casual, natural)

---

## 👤 Author

**Jingtai Chen**  
Undergraduate @ UC Riverside  
[GitHub](https://github.com/Jingtai-Chen)
