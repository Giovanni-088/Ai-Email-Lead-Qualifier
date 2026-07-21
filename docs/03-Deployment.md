# Deployment

## Requirements

- Ubuntu Server
- Docker
- n8n
- Groq API Key
- Telegram Bot
- Gmail SMTP Account

## Environment Variables

```env
Groq_API_KEY=

TELEGRAM_BOT_TOKEN=
TELEGRAM_CHAT_ID=

SMTP_HOST=
SMTP_PORT=
SMTP_USER=
SMTP_PASSWORD=
```

## Services

- n8n
- Groq
- Gmail SMTP
- Google Sheets or NocoDB

## Deployment

Clone the repository and configure the environment variables before importing the n8n workflow.
