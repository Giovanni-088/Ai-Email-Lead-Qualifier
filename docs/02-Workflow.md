# Workflow

## Overview

The workflow automates the complete lead qualification process from form submission to notification.

## Flow

1. Receive form submission through a webhook.
2. Validate required fields.
3. Send the lead information to Groq.
4. Receive AI classification.
5. Classify the lead as:
   - HOT
   - WARM
   - COLD
6. Store the lead information.
7. Send email (HOT only).
8. Send Telegram notification (HOT only).

## Expected Output

- Qualified lead
- Stored record
- Email notification
- Telegram notification
