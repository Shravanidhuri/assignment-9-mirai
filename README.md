# Assignment 9 – AI-Powered Weekly Content Automation (Mirai)

This project demonstrates an automated workflow that generates and publishes AI-driven LinkedIn posts on a weekly basis using Google Sheets, an AI Agent, and external APIs.

The workflow is designed to fetch content ideas from a spreadsheet, enrich them using an AI model, and automatically publish posts while keeping the data source updated.

---

## 🚀 Workflow Overview

The automation runs **every Sunday** and follows these steps:

1. **Weekly Trigger**
   - Initiates the workflow automatically every Sunday.

2. **Fetch Data from Google Sheets**
   - Reads one or more rows from a Google Sheet containing post ideas or prompts.

3. **HTTP Request (Tavily API)**
   - Sends a POST request to fetch additional contextual or research data to enrich the content.

4. **AI Agent Processing**
   - Uses an OpenAI-powered AI Agent to:
     - Understand the input prompt
     - Generate a polished LinkedIn post
     - Structure the output using a structured output parser

5. **Update Google Sheet**
   - Writes the generated content or status back to the same Google Sheet (e.g., marking the row as completed or storing the generated post).

6. **Publish to LinkedIn**
   - Automatically creates and publishes a LinkedIn post using the generated content.

---

## 🧠 Key Features

- Fully automated weekly content creation
- AI-generated LinkedIn posts
- Google Sheets as a simple CMS
- External API integration for enhanced context
- Structured AI output for reliability
- No manual intervention once deployed

---

## 🛠️ Tools & Technologies Used

- Google Sheets (data source & tracking)
- OpenAI Chat Model (AI Agent)
- Tavily API (contextual data retrieval)
- LinkedIn API (post publishing)
- Automation workflow platform (node-based)

---

## 📊 Use Case

This workflow is ideal for:
- Personal branding automation
- Social media managers
- Weekly content pipelines
- AI-driven marketing experiments
- Academic or hackathon assignments

---

## ⚙️ Setup Instructions

1. Create a Google Sheet with post ideas or prompts.
2. Configure API credentials for:
   - OpenAI
   - Tavily
   - LinkedIn
3. Connect each node in the workflow as shown.
4. Set the weekly trigger schedule.
5. Activate the workflow.

---

## 📌 Notes

- Ensure API rate limits are respected.
- The workflow uses structured output parsing to avoid malformed AI responses.
- Google Sheets acts as both input and logging layer.

---

## 📄 License

This project is for educational and demonstration purposes.
