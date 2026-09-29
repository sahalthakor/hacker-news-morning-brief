# 📰 Hacker News Morning Brief

An automated Hacker News morning briefing system built with n8n and Telegram.

The workflow automatically:

1. Fetches Hacker News top stories
2. Selects the top 5 stories
3. Retrieves detailed story information
4. Validates the API response
5. Checks story scores
6. Assigns HIGH/NORMAL priority
7. Builds a formatted morning digest
8. Sends the digest to Telegram

## 🛠️ Tech Stack

- n8n
- Hacker News Firebase API
- JavaScript
- Telegram Bot API

## 🔄 Workflow

Schedule Trigger
↓
HN Top Stories
↓
Select Top 5
↓
HN Story Details
↓
Normalize + Validate
↓
API OK?
↓
Score >= 100?
↓
Mark HIGH / NORMAL
↓
Merge Results
↓
Build Digest
↓
Telegram

## 📸 Screenshots

### Complete Workflow

![Workflow](screenshots/workflow.png)

### Generated Digest

![Build Digest](screenshots/build-digest.png)

### Telegram Output

![Telegram](screenshots/telegram-message.png)

## 🚀 Setup

1. Import `hacker-news-morning-brief.json` into n8n.
2. Create a Telegram Bot using BotFather.
3. Add your Telegram credentials to n8n.
4. Set your Telegram Chat ID.
5. Configure the Schedule Trigger.
6. Activate the workflow.

## 🔐 Security

No API keys, bot tokens, passwords, or private credentials should be committed to this repository.

Credentials should be configured directly inside n8n.

## 📄 License

MIT
