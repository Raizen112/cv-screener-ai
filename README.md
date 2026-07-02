# 🤖 CV Screener AI

An automated CV screening system powered by local AI (LLaMA 3.2 via Ollama) and n8n workflow automation.

## 💡 What it does

- Accepts a candidate name, CV content, and job description via a web form
- Sends the data to a local LLM (LLaMA 3.2) for intelligent analysis
- Returns a structured evaluation with score, strengths, weaknesses, and recommendation
- Saves results automatically to an Excel file

## 🧠 How it works

Form Submission → Basic LLM Chain (Ollama/LLaMA 3.2) → JSON Parser → Excel Output

## 🛠️ Tech Stack

- **n8n** — workflow automation (self-hosted via Docker)
- **Ollama** — local LLM runtime (no API cost, runs fully offline)
- **LLaMA 3.2** — AI model for CV analysis
- **Docker** — containerized environment

## 📊 Output Format

| Nom | Score | Points forts | Points faibles | Recommandation | Date |
|-----|-------|--------------|----------------|----------------|------|

## 🚀 How to run it

1. Install [Docker](https://docker.com) and [Ollama](https://ollama.com)
2. Pull the model: `ollama pull llama3.2`
3. Run n8n: `docker run -it --rm -p 5678:5678 n8nio/n8n`
4. Import the workflow JSON into n8n
5. Open the form URL and submit a CV

## 👤 Author

**Adam Benmoussa** — Engineering Student at ESITH Casablanca
Specialized in Business & Data Management | AI Automation & BI
