# AMRaCS — Agent Mail Reader adds Comments & Summary 🤖📧

An n8n automation workflow that reads incoming code-related emails, summarizes the code, adds inline comments, and sends the result back to you — all automatically using Google Gemini AI.

## 📸 Workflow Preview

![AMRaCS Workflow](screenshot.png)

## 🔧 How It Works

1. **Gmail Trigger** — detects new emails containing code
2. **Parallel Processing:**
   - `comment addition` — generates inline comments for the code
   - `code summary` — summarizes what the code does
3. **Merge & Aggregate** — combines both outputs
4. **Edit Fields** — structures the final output
5. **Basic LLM Chain** — final formatting pass via Gemini
6. **Send a Message** — replies to your Gmail with the result

## 🛠️ Tech Stack

- [n8n](https://n8n.io/) — workflow automation
- Google Gemini API (free tier)
- Gmail (trigger + output)

## 🚀 Setup Instructions

1. Import `workflow.json` into your n8n instance
2. Connect your **Gmail** account in n8n credentials
3. Add your **Google Gemini API key** in the AI model nodes
4. Activate the workflow

## 👤 Author

**Shashank Sharma** — [GitHub](https://github.com/Genius-ShashankSharma)
