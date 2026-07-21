# AI Email Lead Qualifier

## Objective

Automate lead qualification using Artificial Intelligence. When a user submits a form, the system analyzes the information, classifies the lead, stores the data, and automatically triggers follow-up actions.

---

## Architecture

```text
Form
   │
   ▼
n8n Webhook
   │
   ▼
Validation
   │
   ▼
Groq 
   │
   ▼
Classification
   │
   ▼
IF
├── HOT
│   ├── Google Sheets
│   ├── Gmail
│   └── Telegram
├── WARM
│   └── Google Sheets
└── COLD
    └── Google Sheets
```

---

## Technologies

- Ubuntu Server
- Docker
- n8n
- Groq
- Telegram Bot API
- Gmail SMTP
- Google Sheets

---

## Features

- AI-powered lead qualification
- Automatic lead prioritization
- Lead registration
- Email notifications
- Telegram notifications
- Workflow automation
- Webhook-based lead intake

---

## Installation

```bash
git clone <repository-url>
cd AI-Email-Lead-Qualifier
```

---

## Workflow

1. Receive form submission.
2. Validate input data.
3. Analyze the lead with AI.
4. Classify the lead.
5. Store the result.
6. Send notifications.

---

## Screenshots

Coming soon.

---

## Demo

Coming soon.

---

## Roadmap

- [x] Form submission
- [x] Lead input with Google Forms
- [x] AI qualification
- [x] Workflow routing
- [x] Lead storage with Google Sheets
- [x] Automatic email
- [x] Telegram notification
- [ ] Dashboard
