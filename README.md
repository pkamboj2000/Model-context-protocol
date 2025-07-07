# 🎓 MCP University Information Agent

This project uses **LangChain's MCP Agent** with **FastAPI-based tools** to extract key information about U.S. universities such as:
- 🌐 Official university website  
- 📅 Application deadlines and instructions  
- 📊 Computer Science rankings  

It leverages:
- 🛠️ LangChain's `McpAgentExecutor`  
- 🌐 FastAPI + Pydantic for local tools  
- 🧠 OpenAI LLM via `ChatOpenAI`  
- 🧾 BeautifulSoup for HTML text scraping  
- 📊 CollegeScorecard API for university URL resolution

---

## 🚀 Features

| Tool Name                | Description                                                                 |
|--------------------------|-----------------------------------------------------------------------------|
| `get_university_url`     | Gets the official university website using CollegeScorecard API             |
| `extract_deadline_info`  | Extracts top 5 lines from university site containing application keywords   |
| `get_ranking`            | Returns simulated CS rankings (hosted endpoint example)                     |

---

## 📦 Dependencies

Install required libraries with:

```bash
pip install fastapi pydantic requests bs4 langchain openai

