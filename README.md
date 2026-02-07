This workflow automatically monitors incoming Gmail messages and sends notifications to a Slack channel.
It is designed as a simple automation example demonstrating API authentication, triggers, and integrations using n8n.

Features

Monitors new Gmail emails in real time

Extracts message details (sender, subject, preview)

Formats a structured Slack notification

Sends the alert automatically to a selected Slack channel

Workflow Structure
Gmail Trigger → Format Slack Message → Send to Slack

Nodes

Gmail Trigger

Watches for new incoming emails

Authenticated using Gmail OAuth2

Format Slack Message (Set Node)

Extracts:

Subject

Sender

Recipient

Message preview

Message ID

Prepares data for Slack

Send to Slack

Sends a formatted notification to the configured Slack channel using Slack OAuth

Example Slack Message
📧 New Gmail Message

From: sender@example.com
To: receiver@example.com
Subject: Example subject

Preview:
This is a preview of the email message...

Message ID: XXXXX

Setup Instructions

Import the workflow JSON into n8n.

Connect your Gmail OAuth2 credentials.

Connect your Slack OAuth2 credentials.

Select the Slack channel where notifications should be sent.

Activate the workflow.

Use Cases

Important email monitoring

Support inbox alerts

Business notifications

Automated team communication

Future Improvements

Keyword-based filtering

Multiple Slack channels based on rules

Logging alerts to Google Sheets

Priority tagging for urgent messages
