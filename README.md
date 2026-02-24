# ✈️ AI Trip Planner

An intelligent AI-powered travel planning system that generates personalized travel itineraries based on user preferences such as destination, duration and budget.

This project uses an **agent-based LLM workflow** with structured prompt engineering, tool integration, logging and custom exception handling. It includes both a FastAPI backend and a Streamlit frontend.

---

## 🚀 Features

- 🧠 Agent-based AI workflow (LangGraph)
- 📅 Personalized itinerary generation
- 💰 Budget-aware planning
- 🛠️ Tool integration (calculations, helpers)
- 📄 Document generation support
- 📊 Rotating file logging system
- 🚨 Custom exception handling
- 🌐 FastAPI backend
- 🖥️ Streamlit interactive UI

---

# 📂 Folder Structure

```
AI_Trip_Planner/
│
├── agent/               # AI workflow and reasoning logic
├── config/              # Model & application configuration
├── exception/           # Custom exception handling system
├── logger/              # Logging configuration (rotating logs)
├── notebook/            # Development & testing notebooks
├── prompt_library/      # Prompt templates for LLM
├── tools/               # Agent tools (calculations, helpers, etc.)
├── utils/               # Common utility/helper functions
│
├── main.py              # FastAPI backend entry point
├── streamlit_app.py     # Streamlit frontend UI
├── requirements.txt     # Project dependencies
├── pyproject.toml       # Project metadata
└── README.md
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/Rhythm22Sharma/AI_Trip_Planner.git
cd AI_Trip_Planner
```

---

## 2️⃣ Create Virtual Environment (Recommended: UV)

Create environment:

```bash
uv venv env
```

Activate it:

### Windows:
```bash
env\Scripts\activate
```

### Mac/Linux:
```bash
source env/bin/activate
```

---

## 3️⃣ Install Dependencies

Using UV:
```bash
uv pip install -r requirements.txt
```

Or using pip:
```bash
pip install -r requirements.txt
```

---

# 🔐 Environment Variables (.env Setup)

Create a `.env` file in the root directory.

Add the following:

```
GROQ_API_KEY = ""
GOOGLE_API_KEY = ""
GPLACES_API_KEY = ""
FOURSQARE_API_KEY = ""
TAVILY_API_KEY = ""
OPENWEATHER_API_KEY = ""
EXCHANGE_RATE_API_KEY = ""
ALPHAVANTAGE_API_KEY = ""
```


# 🚀 Running the Application

You need to start **both backend and frontend**.

---

## 🔹 1️⃣ Start FastAPI Backend

Run:

```bash
uvicorn main:app --reload --port 8000
```

Backend will run at:

```
http://127.0.0.1:8000
```

Swagger API Documentation:

```
http://127.0.0.1:8000/docs
```

---

## 🔹 2️⃣ Start Streamlit Frontend

Open a new terminal (keep backend running).

Run:

```bash
streamlit run streamlit_app.py
```

The Streamlit UI will open automatically in your browser.

---

# 🧠 How It Works (Architecture Overview)

```
User
  ↓
Streamlit UI
  ↓
FastAPI Backend
  ↓
Agent Workflow (LangGraph)
  ↓
LLM + Tools
  ↓
Generated Itinerary
```

### System Components

- **Agent** → Controls AI reasoning workflow  
- **Prompt Library** → Structured LLM prompts  
- **Tools** → Extend LLM capabilities  
- **Utils** → Reusable helper functions  
- **Logger** → Rotating file logging system  
- **Exception Module** → Custom error handling  





# 🛠️ Tech Stack

- Python
- FastAPI
- Streamlit
- LangGraph
- LangChain
- OpenAI / LLM
- UV (Package Manager)
- Logging & Exception Handling

---

# 📌 Future Improvements

- Add hotel/flight API integration
- Export itinerary as PDF
- Deploy on cloud (Render / AWS / Azure)
- Add user authentication
- Add caching for performance

---

# 📄 License

This project is built for educational and portfolio purposes.

---

# 👨‍💻 Author

**Rhythm Sharma**  
🎓 Computer Science Engineer  

🔗 GitHub: [Rhythm Sharma](https://github.com/Rhythm22Sharma)

