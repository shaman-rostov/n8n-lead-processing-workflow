# Workflow Logic Overview

## Trigger
- Google Sheets Trigger
- Fires instantly when a new form response is submitted

## Step 1: Edit Fields Node
- Normalize field names
- Convert dates, phone numbers, and names to unified formats
- Prepare structured JSON for all integrations

## Step 2: Trello Task
- Create a card on a selected board & list
- Include client info, request details, deadline
- Apply labels according to request type

## Step 3: Telegram Notification
- Sends team message instantly
- Contains lead details and link to Trello card

## Step 4: Google Calendar Reminder
- Creates an event with follow-up date or deadline
- Ensures no task is forgotten

## Step 5: Agile CRM Contact
- Adds lead to CRM
- Tags with lead source ("Google Form")
- Prepares for future automations (emails, funnels, workflows)

## Design Principles
- Idempotent execution
- Fail-safe handling
- Data never lost or corrupted
- Minimal API calls
