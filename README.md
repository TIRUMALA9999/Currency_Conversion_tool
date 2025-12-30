# Currency Conversion Tool — Agentic AI Tooling with CrewAI

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![CrewAI](https://img.shields.io/badge/CrewAI-Tooling-black)
![API](https://img.shields.io/badge/API-Currency%20Rates-green)

**Target audience:** Recruiters / Hiring Managers  
**Style:** Resume‑focused • Interview‑explainable • ATS‑friendly  

This project demonstrates how to build a **tool‑augmented LLM agent** using **CrewAI** to perform **real‑time currency conversion** by calling an external exchange‑rate API.

---

## Key highlights (30‑second recruiter summary)

- Built a **custom CrewAI tool** for live currency conversion using an external REST API.
- Integrated the tool into an **LLM-powered agent** that decides when to call the API.
- Demonstrates **tool calling**, **API integration**, and **agent reasoning**.
- Implemented in clean, reproducible **Jupyter notebooks**.

**ATS keywords:** LLM agents, CrewAI, tool calling, API integration, Python, REST APIs, currency conversion, agentic AI.

---

## What this project shows

### Agent + Tool Pattern
- An LLM agent receives a user query (e.g., *“Convert 100 USD to INR”*).
- The agent invokes a **custom tool** that:
  - Calls a currency exchange API
  - Fetches live conversion rates
  - Returns structured results
- The agent formats and explains the output to the user.

This mirrors **real-world AI systems** where LLMs orchestrate external tools rather than hallucinating data.

---

## Repository structure

```
Currency_Conversion_tool-main/
├─ notebook.ipynb      # Core currency conversion agent + tool
└─ notebook1.ipynb     # Extended / alternative implementation
```

---

## Tech stack

- **Python**
- **CrewAI**
  - Agent
  - Task
  - Custom Tool (`BaseTool`)
- **requests** (external API calls)
- **pydantic** (input/output validation)
- **dotenv** (environment variables)
- **Jupyter Notebook**

---

## How to run locally

### 1) Clone
```bash
git clone https://github.com/<your-username>/Currency_Conversion_tool.git
cd Currency_Conversion_tool
```

### 2) Create environment
```bash
python -m venv .venv
.venv\Scripts\activate   # Windows
# or
source .venv/bin/activate # macOS/Linux
```

### 3) Install dependencies
```bash
pip install crewai requests python-dotenv pydantic jupyterlab
```

### 4) Configure environment variables
Create a `.env` file:
```env
API_KEY=your_currency_api_key
```

### 5) Run notebooks
```bash
jupyter lab
```
Open `notebook.ipynb` and run all cells.

---

## Interview talking points

- “I implemented a **custom CrewAI tool** to fetch live currency rates instead of relying on static data.”
- “This project shows how LLMs can **reason about when to call APIs** rather than hallucinating answers.”
- “I used **Pydantic models** to validate tool inputs and outputs for reliability.”
- “This pattern is directly transferable to finance, travel, and e‑commerce systems.”

---

## Possible extensions

- Add support for historical exchange rates
- Cache frequent conversions
- Add error handling & retry logic
- Convert notebooks into a CLI or FastAPI service
- Add unit tests for the tool logic

---

## Author

**Tirumala Teja Yegineni**  
GitHub: https://github.com/TIRUMALA9999
