# Architecture

## Objective

Automatically qualify incoming leads using Artificial Intelligence.

## System Architecture

```text
Form
   │
   ▼
Webhook
   │
   ▼
Validation
   │
   ▼
OpenAI
   │
   ▼
Classification
   │
   ▼
IF
├── HOT
│   ├── Store Lead
│   ├── Send Email
│   └── Send Telegram Notification
├── WARM
│   └── Store Lead
└── COLD
    └── Store Lead
```

## Components

- n8n
- Groq API (Llama 3.x)
- Google Sheets
- Gmail SMTP
- Telegram Bot API
