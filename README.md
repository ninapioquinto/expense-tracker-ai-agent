#  Expense Tracker AI Agent

An AI-powered workflow built with n8n and LangChain to track your expenses from natural language chat inputs. It extracts structured data (cost, description, date) and logs it into Google Sheets.

---

##  Overview

This project aims to simplify expense tracking by enabling users to interact with a chatbot using natural language. Instead of manually entering expenses into a spreadsheet or app, users can simply say something like:

> "I spent $1000 on a business conference in New York."

The system interprets the message, extracts the key information, and saves it in a structured format to Google Sheets, all automatically and in real time.

---

##  Features

-  **AI Agent**: Uses OpenAI's GPT to interpret expense messages.
-  **Google Sheets Integration**: Automatically logs parsed expenses to a spreadsheet.
-  **LangChain Tools**: Modular memory, tools, and agent support.

---

##  Requirements

- n8n
- Google Sheets credentials
- OpenAI API key
- LangChain Nodes

---

##  Workflow Overview

| Component                          | Role                                                                 |
|-----------------------------------|----------------------------------------------------------------------|
| `AI Agent`                        | Handles chat messages and invokes tools                             |
| `When chat message received`      | Trigger for new messages                                             |
| `Expense text to JSON parser`     | Parses unstructured text into cost, date, and description           |
| `Save expense into Google Sheets` | Writes parsed data to a spreadsheet                                 |
| `Parse msg and save to Sheets`    | LangChain tool integration with sub-workflow support                |

---

##  Use Case

- **Service-Based Business Owners**: Quickly log daily expenses via chat without disrupting workflow.
- **Startup Teams**: Integrate in Slack or a custom UI for streamlined internal expense tracking.
- **Productivity Hackers**: Automate routine financial logging using AI and low-code automation.

It’s especially useful when paired with other workflows, such as monthly report generation or integration with financial dashboards.


##  File Contents

- `Expense_Tracker_AI_Agent.json`

---

##  Created by Nina Pioquinto

Automation Systems Engineer    
Helping businesses scale smart systems with ai automation and crm solutions.

> Let’s build your custom system
