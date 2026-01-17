📬 AI-Powered Professional Email Reply Agent (for TUITION NEPAL)
🧠 Overview
This repository contains a complete n8n workflow that automatically reads Gmail messages and replies professionally using Google Gemini AI.
It’s tailored for Sangita Sharma of TUITION NEPAL.

📁 Project Structure
n8n-email-ai-agent/
├── agents/
│   ├── professional_email.json   # The n8n workflow
│   └── email_prompt.json         # The AI prompt instruction set
├── screenshots/
│   └── workflow-preview.png
├── README.md
├── .gitignore
└── LICENSE
The AI prompt logic (including tone rules and examples) is stored in agents/email_prompt.json.

⚙️ Workflow Overview
Node	Description
Schedule Trigger	Checks for new unread emails every minute.
Gmail (getAll)	Fetches unread messages.
Gmail (get details)	Retrieves email contents.
AI Agent (Gemini)	Drafts the reply using the instruction prompt.
Mark as Read	Marks the email as processed.
Reply to Message	Sends the generated reply.
Airtable	Logs all details.
Workflow Preview

🚀 Setup Instructions
Import the workflow

Open n8n
Go to Workflows → Import
Select agents/professional_email.json
Configure credentials

Gmail OAuth2
Google Gemini API key
Airtable personal access token
Activate the workflow

Toggle “Active” in n8n
🧠 AI Prompt
The full configuration that defines how the AI behaves is available in:

agents/email_prompt.json
This defines tone handling, structure, signature, and examples for the AI reply style.

🧩 Stack
n8n Automation
Google Gemini AI
Gmail API
Airtable API
📄 License
MIT License – see LICENSE

AI_AGENT_EMAILREPLY
