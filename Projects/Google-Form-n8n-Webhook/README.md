# Google Form to n8n Webhook

## Project Overview

This project connects Google Forms with n8n using Google Apps Script and ngrok.

When a user submits a Google Form, the form data is automatically sent to an n8n webhook, which can then trigger further automation workflows.

## Workflow

Google Form
→ Google Apps Script
→ ngrok
→ n8n Webhook

## Technologies Used

- Google Forms
- Google Apps Script
- ngrok
- n8n

## Challenges Faced

### 1. localhost not accessible
Google Apps Script runs on Google's servers and cannot access localhost directly.

### Solution
Used ngrok to expose the local n8n instance to the internet.

### 2. Trigger configuration issue
The trigger was initially set to "On Open" instead of "On Form Submit".

### Solution
Changed the trigger to "On Form Submit".

## Outcome

Successfully triggered an n8n workflow whenever a Google Form was submitted.

## Key Learnings

- How webhooks work
- Google Apps Script triggers
- Why localhost cannot be accessed externally
- Using ngrok for local development
- Connecting Google services with n8n
