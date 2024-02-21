# AITH-bot
Chatbot for AI Talent Hub ITMO students

# Usage
## Overview of my courses
Upon setup, Generates a message/messages with links to notion / chats / google drive / any other relevant sources 
for each course. Also includes dates and schedule.

> Alternatively, a separate page with info on each course

## Timetable

Perhaps [previous work](https://github.com/Samoed/itmo-ai-timetable-ics/tree/main) can be implemented for parsing?

- Today
- Tomorrow
- all days (this week or in general if schedule is stable)

## Notifications
- before lesson (customisable)
- weekly / daily schedule sending
- special events (meetups etc)

# Other
- Link to talent-matcher website on main page / project seminar page
- Link to this git page / Buymeacoffee / contact info
- Suggest features

---

#### Collab with DS-jr
- Track relevant stuff (either via tags (messages from admins, with regexp), or with plain-text (using NLP + maybe small LLM))
    relevancy can be based on user's course choice. Tracking should be customisable (make a page with selection)
- Summarizer for flood topics

---

# Stack
- [aiogram](https://docs.aiogram.dev/en/latest/) for Telegram client, because I want to learn it + it might be slightly faster than Telebot
- sqlite for databases
- Google Sheets as data source + [gspread](https://github.com/burnash/gspread) for API
- Docker for deployment

# Misc
Need to discuss integrating with hub