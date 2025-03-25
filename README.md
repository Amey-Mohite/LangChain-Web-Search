
# 🔎 LangChain Chatbot with Web Search

A Streamlit-powered chatbot that uses **LangChain agents**, **Groq’s ultra-fast LLaMA 3 model**, and popular tools like **Wikipedia**, **Arxiv**, and **DuckDuckGo Search** to intelligently answer your questions in real-time. ✨

> 📘 *Inspired by the [Complete Generative AI Course with LangChain and HuggingFace](https://www.udemy.com/course/complete-generative-ai-course-with-langchain-and-huggingface/learn/lecture/44599733?start=585) on Udemy.*

---

## 🚀 Features

- 🧠 **LangChain Zero-Shot Agent** for tool-based reasoning
- 🔍 **Tool Integration**:
  - Wikipedia summaries
  - Arxiv academic paper lookup
  - DuckDuckGo web search
- ⚡ **Groq LLM (LLaMA3-8B-8192)** for blazing-fast responses
- 💬 **Chat UI** with streaming responses via Streamlit
- 🔐 API key input with secure password field in sidebar

---

## 📷 Preview

![demo](https://langchain-web-search-3eflcdw8gny3uztzf8bcc6.streamlit.app/)

---

## 🛠️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Amey-Mohite/langchain-streamlit-chatbot.git
cd langchain-streamlit-chatbot
```

### 2. Create a virtual environment (optional)

```bash
python -m venv venv
source venv/bin/activate  # or .\\venv\\Scripts\\activate on Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Add your Groq API key

You can either:
- Enter the API key in the sidebar at runtime, OR
- Create a `.env` file and add:

```
GROQ_API_KEY=your_groq_api_key
```

---

## 🚦 Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

Then open the URL displayed in your terminal (typically http://localhost:8501).

---

## 📁 Project Structure

```
├── app.py               # Main Streamlit app with LangChain agent logic
├── requirements.txt     # Python dependencies
├── .env (optional)      # Contains your GROQ_API_KEY
└── README.md            # You're reading it :)
```

---

## ✅ Requirements

- Python 3.8+
- [Groq API Key](https://console.groq.com/)

---

## 🧠 How It Works

This app uses a LangChain `ZeroShotAgent` that selects between:
- **DuckDuckGo** for general web queries
- **Wikipedia** for encyclopedia-style lookups
- **Arxiv** for academic content

The LLM (LLaMA 3 hosted on Groq) interprets user input, plans actions using tools, and streams the response back into the chat.

---

## 📚 Reference

- 🎓 [Udemy Course: Complete Generative AI Course with LangChain & HuggingFace](https://www.udemy.com/course/complete-generative-ai-course-with-langchain-and-huggingface/learn/lecture/44599733?start=585)

---

## 🧩 Built With

- [LangChain](https://www.langchain.com/)
- [Streamlit](https://streamlit.io/)
- [Groq](https://groq.com/)
- [DuckDuckGo Search](https://duckduckgo.com/)
- [Wikipedia API](https://www.mediawiki.org/wiki/API:Main_page)
- [Arxiv API](https://arxiv.org/help/api/index)
