# 🤖 Multi-Agent Research Platform

An AI-powered research platform that uses **multiple specialized agents** to search the web, analyze information, and generate structured research reports from a user-provided topic.

## 🚀 Live Demo

🔗 **[Multi-Agent Research Platform](https://multi-agent-research-platform.onrender.com)**

## 📂 GitHub Repository

🔗 **[GitHub Repository](https://github.com/2k23cs2313652-rishi/Multi-Agent-Research-Platform)**

---

## ✨ Features

* 🔍 **Web Research** – Searches the web for relevant information using Tavily.
* 🤖 **Multi-Agent Workflow** – Uses specialized AI agents for different research tasks.
* 📄 **Content Extraction** – Scrapes and extracts useful information from web pages.
* ✍️ **AI Report Generation** – Produces structured and detailed research reports.
* 🧐 **Report Criticism** – Evaluates the generated report and provides improvement suggestions.
* 📚 **Source Collection** – Includes research URLs in the final report.
* 🖥️ **Streamlit Interface** – Simple and interactive web interface.
* ⚡ **Mistral AI** – Uses Mistral models through LangChain.

---

## 🏗️ Architecture

```text
                    User Query
                        │
                        ▼
              ┌──────────────────┐
              │   Search Agent   │
              │   Tavily Search  │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │   Reader Agent   │
              │ Web Page Scraper │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │   Writer Agent   │
              │ Mistral + Prompt │
              └────────┬─────────┘
                       │
                       ▼
              ┌──────────────────┐
              │   Critic Agent   │
              │ Report Evaluation│
              └────────┬─────────┘
                       │
                       ▼
                Final Research
                    Report
```

---

## 🛠️ Tech Stack

| Technology        | Purpose                             |
| ----------------- | ----------------------------------- |
| **Python**        | Core programming language           |
| **LangChain**     | Agent and LLM orchestration         |
| **Mistral AI**    | Large Language Model                |
| **Streamlit**     | Web application interface           |
| **Tavily**        | Web search                          |
| **BeautifulSoup** | Web scraping and content extraction |
| **Requests**      | HTTP requests                       |
| **python-dotenv** | Environment variable management     |

---

## 📁 Project Structure

```text
Multi-Agent-Research-Platform/
│
├── app.py                  # Streamlit application
├── agents.py               # AI agents and LLM chains
├── pipeline.py             # Research workflow
├── tools.py                # Search and scraping tools
├── requirements.txt        # Project dependencies
├── .gitignore
└── README.md
```

---

## 🔄 How It Works

### 1. User enters a topic

The user provides a research topic through the Streamlit interface.

### 2. Search Agent

The Search Agent uses **Tavily Search** to find relevant web sources.

### 3. Reader Agent

The Reader Agent uses the scraping tools to extract useful information from the discovered web pages.

### 4. Writer Agent

The collected research is passed to a **Mistral AI model**, which generates a structured report containing:

* Introduction
* Key Findings
* Conclusion
* Sources

### 5. Critic Agent

The generated report is reviewed by another AI chain that identifies:

* Strengths
* Areas for improvement
* Overall score

### 6. Final Output

The completed research report and critique are displayed through the Streamlit application.

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/2k23cs2313652-rishi/Multi-Agent-Research-Platform.git
cd Multi-Agent-Research-Platform
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

**Windows PowerShell:**

```powershell
.venv\Scripts\Activate.ps1
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file in the project root:

```env
MISTRAL_API_KEY=your_mistral_api_key
TAVILY_API_KEY=your_tavily_api_key
```

> ⚠️ Never upload your `.env` file or API keys to GitHub.

---

## ▶️ Run the Application

Start the Streamlit application with:

```bash
streamlit run app.py
```

The application will open in your browser.

---

## 📊 Example Workflow

```text
Research Topic
      ↓
Tavily Web Search
      ↓
Relevant Sources
      ↓
Web Content Extraction
      ↓
Mistral AI Analysis
      ↓
Structured Research Report
      ↓
AI Critique
      ↓
Final Result
```

---

## 🎯 Project Objective

The goal of this project is to demonstrate how **LLMs, AI agents, web search, web scraping, and prompt engineering** can be combined to build an automated research system.

Instead of manually searching multiple websites and organizing information, the platform automates the research workflow and produces a structured report.

---

## 🔮 Future Improvements

* Add more specialized research agents
* Improve source verification
* Add PDF report export
* Add research history
* Add citation formatting
* Add support for additional LLM providers
* Improve parallel research execution
* Add advanced source ranking

---

## 👨‍💻 Author

**Rishi Gupta**

B.Tech Computer Science & Engineering
Pranveer Singh Institute of Technology, Kanpur

### 🔗 Links

* **GitHub:** [2k23cs2313652-rishi](https://github.com/2k23cs2313652-rishi)
* **Live Project:** [Multi-Agent Research Platform](https://multi-agent-research-platform.onrender.com)

---

⭐ If you find this project useful, consider giving the repository a star!
