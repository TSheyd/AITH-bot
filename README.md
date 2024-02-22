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
### Bot
- [Aiogram](https://docs.aiogram.dev/en/latest/) for Telegram client
- Sqlite for databases
- Docker for deployment

### Integrations
- Google Sheets as data source + [gspread](https://github.com/burnash/gspread) for API

- Notion + Notion API for courses info and other content. **Connecting Notion**:
  1. Go to https://www.notion.so/my-integrations/ and click on "New integration".
  2. Fill in the name of the integration, select the workspace and click "Submit".
  3. In "Capabilities" select only "Read content" in Content capabilities and "No user information" in User capabilities, click "Save changes".
  4. **Go to the Courses page**, click ... → Connect to → Find the created connection → Select → Confirm.
  5. Copy the "Internal Integration Secret" and paste it into the config file.
