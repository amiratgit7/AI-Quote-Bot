# AI Motivational Quote Bot

An automated AI agent that generates and delivers a fresh motivational quote to your email every morning using Groq AI and n8n.

## How It Works

```
Schedule Trigger (8 AM daily)
        ↓
Groq AI — LLaMA 3.3 70B generates a motivational quote
        ↓
Format Message — adds date and greeting
        ↓
Gmail — delivers the quote to your inbox
```

## Tech Stack

| Tool | Purpose |
|------|---------|
| [n8n Cloud](https://n8n.io) | Workflow automation platform |
| [Groq API](https://console.groq.com) | AI inference — LLaMA 3.3 70B model |
| Gmail API (OAuth2) | Email delivery |

## Features

- Runs automatically every morning at 8:00 AM
- Generates a unique quote daily using a large language model
- Delivers to one or multiple email addresses
- Zero manual effort after setup — fully autonomous

## Sample Output

```
Subject: Your Morning Motivational Quote

Good Morning!

"Believe you can and you're halfway there." - Theodore Roosevelt

Date: Tuesday, May 12, 2026

Have an amazing day ahead!
```

## Project Structure

```
AIQuoteBot/
├── workflow/
│   └── motivational_quote_bot.json   ← n8n workflow
├── screenshots/
│   ├── workflow.png                   ← n8n workflow screenshot
│   └── email_sample.png              ← sample email received
├── SETUP_GUIDE.md                     ← full setup instructions
└── README.md                          ← this file
```

**Requirements:**
- n8n Cloud account (free trial at n8n.io)
- Groq API key (free at console.groq.com)
- Gmail account

## Skills Demonstrated

- AI/LLM integration (Groq API, LLaMA 3.3 70B)
- Workflow automation (n8n)
- REST API usage (HTTP requests, OAuth2)
- Scheduled automation (cron expressions)
- End-to-end autonomous agent design

## Author

**Amir** — Built and deployed independently using n8n Cloud and Groq AI.
