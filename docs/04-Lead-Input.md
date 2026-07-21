# Lead Input

## Objective

Create the entry point for incoming leads and send the information to n8n through a webhook.

## Input Method

The system uses Google Forms to collect lead information.

Each submission is automatically stored in Google Sheets.

n8n monitors the spreadsheet and retrieves new rows as soon as they are created, triggering the lead qualification workflow.

## Lead Fields

The form will send the following fields:

| Field | Description |
|---|---|
| name | Lead full name |
| email | Contact email |
| company | Company name |
| position | Job position |
| message | Lead description |
| budget | Estimated budget |

## Data Flow

```text
Form
 │
 ▼
HTTP POST Request
 │
 ▼
n8n Webhook
 │
 ▼
JSON Payload

Example Payload
{
  "name": "John Smith",
  "email": "john@example.com",
  "company": "Example Corp",
  "position": "Manager",
  "message": "Interested in automation services",
  "budget": "$5000"
}
Validation

Required fields:

name
email
message

The workflow must reject incomplete submissions.

Verification

A successful test must show the received JSON inside the n8n Webhook node.
