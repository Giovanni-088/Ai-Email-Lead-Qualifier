# Architecture

## Objective

Automatically qualify incoming leads using Artificial Intelligence.

## System Architecture

```text
Google Form
        │
        ▼
Google Sheets
        │
        ▼
n8n
        │
        ▼
Groq (Llama 3.3)
        │
        ▼
JSON Parse
        │
        ▼
Routing
 ┌──────────────┬──────────────┬──────────────┐
 ▼              ▼              ▼
HOT           WARM          COLD
 │              │              │
 └──────────────┴──────────────┘
               │
               ▼
Google Sheets (Qualified Leads)
               │
        ┌──────┴──────┐
        ▼             ▼
 Gmail SMTP     Telegram Bot

Any Failure
      │
      ▼
Error Trigger
      │
      ├── Workflow Errors (Google Sheets)
      └── Telegram Alert
```

## Components

- n8n
- Groq API (Llama 3.x)
- Google Sheets
- Gmail SMTP
- Telegram Bot API
