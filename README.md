# 🤖 AI Appointment Scheduling and Reminder Agent

An AI-powered appointment scheduling and reminder automation system built using **n8n**, **Groq LLM**, **Google Gemini**, **WhatsApp Cloud API**, **Google Calendar API**, **Google Sheets API**, and **Gmail API**.

The system allows users to book appointments through WhatsApp using natural language. It intelligently checks calendar availability, schedules appointments, stores patient information, sends confirmation emails and WhatsApp messages, and automatically delivers reminder notifications before the scheduled appointment.

---

## 🚀 Features

- 🤖 AI-powered appointment booking using Groq LLM
- 💬 Natural language interaction via WhatsApp
- 📅 Google Calendar availability checking
- 📆 Automatic Google Calendar event creation
- 📋 Appointment data storage in Google Sheets
- 📧 Automated Gmail confirmation emails
- 📲 WhatsApp confirmation messages
- ⏰ Intelligent reminder workflow powered by Google Gemini
- 🧠 AI conversation memory for better interactions
- ⚡ End-to-end workflow automation using n8n

---

# 🏗️ Architecture

```
                    User
                      │
                      ▼
             WhatsApp Cloud API
                      │
                      ▼
             WhatsApp Trigger (n8n)
                      │
                      ▼
             AI Agent (Groq LLM)
             ┌────────┼───────────┐
             │        │           │
             ▼        ▼           ▼
     Check Calendar  Create Event  AI Memory
             │
             ▼
     Google Calendar API
             │
             ▼
     Google Sheets API
             │
     ┌───────┴─────────┐
     ▼                 ▼
 Gmail API      WhatsApp Reply


──────────────────────────────────────────────

          Reminder Automation

     Schedule Trigger (n8n)
             │
             ▼
      Google Sheets API
             │
             ▼
     JavaScript Processing
             │
             ▼
     Google Gemini LLM
             │
             ▼
       Gmail Reminder
             │
             ▼
 Update Reminder Status
```

---

# 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------|
| Workflow Automation | n8n |
| AI Models | Groq LLM, Google Gemini |
| Programming | Python, JavaScript |
| Database | Google Sheets |
| Calendar | Google Calendar API |
| Email | Gmail API |
| Messaging | WhatsApp Cloud API |
| Integration | REST APIs |

---

# 📂 Project Structure

```
AI-Appointment-Scheduling-Agent/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── workflow/
│   ├── appointment-agent.json
│   └── reminder-agent.json
│
├── screenshots/
│   ├── appointment-workflow.png
│   ├── reminder-workflow.png
│   ├── gmail-confirmation.png
│   ├── whatsapp-demo.png
│   └── google-calendar.png
│
└── docs/
    └── architecture.png
```

---

# 🔄 Workflow Overview

## 1️⃣ Appointment Scheduling Workflow

The appointment scheduling workflow enables users to book appointments directly through WhatsApp.

### Workflow Steps

1. User sends an appointment request on WhatsApp.
2. Groq-powered AI Agent understands the request.
3. Calendar availability is checked.
4. Appointment is created in Google Calendar.
5. Patient details are stored in Google Sheets.
6. Confirmation email is sent using Gmail.
7. WhatsApp confirmation message is delivered to the user.

---

## 2️⃣ Reminder Workflow

The reminder workflow runs automatically at scheduled intervals.

### Workflow Steps

1. Schedule Trigger starts the workflow.
2. Reads appointment records from Google Sheets.
3. Filters upcoming appointments.
4. JavaScript processes appointment data.
5. Google Gemini generates reminder content.
6. Reminder email is sent via Gmail.
7. Google Sheets is updated to prevent duplicate reminders.

---

# 📸 Screenshots

## Appointment Scheduling Workflow

> Add screenshot here

```
screenshots/appointment-workflow.png
```

---

## Reminder Workflow

> Add screenshot here

```
screenshots/reminder-workflow.png
```

---

## Gmail Confirmation

> Add screenshot here

```
screenshots/gmail-confirmation.png
```

---

## WhatsApp Appointment Booking

> Add screenshot here

```
screenshots/whatsapp-demo.png
```

---

## Google Calendar Event

> Add screenshot here

```
screenshots/google-calendar.png
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/Adityagsh/AI-Appointment-Scheduling-Agent.git
```

Move into the project directory.

```bash
cd AI-Appointment-Scheduling-Agent
```

---

## Import Workflows

Import the following workflows into your n8n workspace.

- workflow/appointment-agent.json
- workflow/reminder-agent.json

---

## Configure Credentials

Create credentials for:

- Groq API
- Google Gemini API
- WhatsApp Cloud API
- Google Calendar API
- Google Sheets API
- Gmail API

---

## Activate Workflows

Enable both workflows in n8n.

Start chatting with your WhatsApp bot to schedule appointments.

---

# 📈 Future Improvements

- Voice-based appointment booking
- Doctor/Admin dashboard
- SMS reminders
- Patient authentication
- Multi-language support
- MongoDB database integration
- RAG-powered hospital knowledge base
- Analytics dashboard
- PDF appointment reports

---

# 💡 Key Highlights

- AI-powered conversational appointment booking
- Intelligent reminder generation
- Multi-LLM architecture (Groq + Google Gemini)
- Google Calendar integration
- WhatsApp automation
- Email automation
- Google Sheets as backend database
- Python and JavaScript custom processing
- Modular n8n workflows
- Scalable workflow automation

---

# 👨‍💻 Author

### Aditya Sharma

Electronics & Telecommunication Engineer | AI Automation Developer | Python Developer

📧 Email:adityagsh45@gmail.com

🔗 LinkedIn:www.linkedin.com/in/aditya-sharma-147276263

💻 GitHub: https://github.com/Adityagsh

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

Feedback and contributions are always welcome.
