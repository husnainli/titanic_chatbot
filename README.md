# 🚢 Titanic Data Analyst Chatbot

[![Made with Streamlit](https://img.shields.io/badge/Made%20with-Streamlit-FF4B4B?logo=streamlit\&logoColor=white)](https://streamlit.io/)
[![Powered by OpenAI](https://img.shields.io/badge/Powered%20by-OpenAI-10a37f?logo=openai\&logoColor=white)](https://openai.com/)
[![App is Live](https://img.shields.io/badge/🚀%20App%20Live-Click%20Here-brightgreen)](https://titanic-chatbot-dashboard.streamlit.app)
[![GitHub stars](https://img.shields.io/github/stars/husnainli/titanic_chatbot?style=social)](https://github.com/husnainli/titanic_chatbot)
[![MIT License](https://img.shields.io/github/license/husnainli/titanic_chatbot)](LICENSE)

An intelligent, interactive Streamlit app that allows users to explore the Titanic dataset using natural language questions. The app leverages OpenAI's GPT API to interpret queries, generate Python code, execute it, and return visual or textual insights — just like a real data analyst!

🔗 **Live Demo:** [https://titanic-chatbot-dashboard.streamlit.app](https://titanic-chatbot-dashboard.streamlit.app)

---

## ✨ Features

* **LLM-powered chatbot** to explore Titanic data using natural language
* Auto-generated **charts** using Plotly and Matplotlib
* Sidebar-based **data filters** and interactive visual explorer
* **Chat history** and intelligent **follow-up suggestions**
* Modular, maintainable, component-based structure
* Fully deployed on **Streamlit Cloud**

---

## 📁 Project Structure

```
titanic_chatbot/
├── app.py                          # Main Streamlit app entrypoint
├── requirements.txt                # Python dependencies
├── .env.example                    # Template for required secrets
├── styles/
│   └── layout.css                  # Custom layout & spacing
├── utils/
│   ├── data.py                     # Load & clean Titanic dataset
│   ├── state.py                    # Session state initializer
│   ├── executor.py                 # Code execution logic
│   ├── llm_handler.py              # OpenAI API interactions
│   └── prompts.py                  # Prompt templates for GPT
├── components/
│   ├── sidebar.py                  # Sidebar filters (class, sex, etc.)
│   ├── chat_history.py             # Previous Q&A display
│   ├── right_panel.py              # Follow-up suggestions
│   ├── chart_explorer.py           # Exploratory chart UI
│   └── question_input.py           # Main user input handler
└── .env                            # Your OpenAI key (not committed)
```

---

## 🚀 Quick Start (Run Locally)

### 1. Clone the Repository

```bash
git clone https://github.com/husnainli/titanic_chatbot.git
cd titanic_chatbot
```

### 2. Add Environment Variables

Create a `.env` file in the root:

```env
OPENAI_API_KEY=your-api-key-here
```

Or copy from template:

```bash
cp .env.example .env
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Start the App

```bash
streamlit run app.py
```

---

## 🌐 Deploy to Streamlit Cloud

This app is already live:
👉 **[https://titanic-chatbot-dashboard.streamlit.app](https://titanic-chatbot-dashboard.streamlit.app)**

To deploy your own:

1. Push your code to a GitHub repo
2. Go to [https://streamlit.io/cloud](https://streamlit.io/cloud)
3. Click **"New App"**, select your repo and `app.py`
4. Go to **Settings → Secrets** and add:

```toml
OPENAI_API_KEY = "your-api-key"
```

5. Click **Deploy**

---

## 📦 Requirements

Contents of `requirements.txt`:

```txt
streamlit
pandas
plotly==5.22.0
matplotlib
seaborn
openai
python-dotenv
```

Install them with:

```bash
pip install -r requirements.txt
```

---

## 💬 Example Questions to Try

Ask the chatbot:

* "How many passengers survived?"
* "What is the survival rate by gender?"
* "Plot a bar chart of class distribution"
* "Average age of survivors?"
* "How many children were on board?"

---

## 🔒 Security Notes

* `.env` is ignored via `.gitignore`
* `.env.example` shows the required keys without revealing yours
* Streamlit Cloud encrypts your secrets automatically

---

## 👨‍💻 Author

**Husnain Ali**
Data Science & AI Enthusiast
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin\&logoColor=white)](https://www.linkedin.com/in/husnainli)

---

## 📝 License

This project is licensed under the [MIT License](LICENSE) — free to use, modify, and share.

---