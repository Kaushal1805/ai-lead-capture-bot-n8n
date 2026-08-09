# 🤖 AI Lead Capture Bot – n8n Automation

An AI-powered lead capture automation built with **n8n, Telegram, and Google Sheets**.

This workflow automatically collects lead information through Telegram, processes the captured data, stores it in a Google Sheets CRM, and sends a confirmation message back to the user.

## 🚀 Project Overview

The goal of this project is to automate the lead collection process for businesses.

Instead of manually collecting customer information, the bot automatically:

1. Receives a message from a potential customer through Telegram.
2. Collects lead information such as name, requirement, and budget.
3. Processes and structures the lead data.
4. Creates or updates a record in Google Sheets.
5. Sends a confirmation message to the customer.

## 🔄 Workflow

```text
Telegram User
      ↓
Telegram Trigger
      ↓
Collect Lead Details
      ↓
Build / Structure Lead Data
      ↓
Google Sheets CRM
      ↓
Telegram Confirmation
```

## 🛠️ Tech Stack

* n8n
* Telegram Bot API
* Google Sheets
* JavaScript
* Workflow Automation
* AI-based Data Processing

## ✨ Features

* 🤖 Automated lead collection
* 📱 Telegram-based interaction
* 🧠 Structured lead data processing
* 📊 Google Sheets CRM integration
* 🔄 Append or update existing leads
* ✅ Automatic confirmation message
* ⚡ No manual data entry required

## 📋 Lead Information Captured

The workflow stores:

| Field       | Description                     |
| ----------- | ------------------------------- |
| Date        | Date when the lead was captured |
| Name        | Lead/customer name              |
| Requirement | Customer requirement            |
| Budget      | Customer budget                 |
| Status      | Current lead status             |

The workflow maps these fields into Google Sheets and uses the lead name as the matching column for append/update operations.

## 🔧 n8n Workflow Nodes

### 1. Telegram Trigger

Receives incoming Telegram messages and starts the automation.

### 2. Collect Lead Details

Processes the incoming information and prepares structured lead data.

### 3. Build Row

JavaScript code structures the lead information before sending it to the CRM.

Example fields:

```javascript
{
  name,
  requirement,
  budget,
  date,
  status
}
```

### 4. Google Sheets CRM

The workflow appends or updates lead information in Google Sheets.

### 5. Send Confirmation

After successfully processing the lead, the bot sends a confirmation message to the customer.

Example:

> Thanks! ✅ We've recorded your request. Our team will contact you soon.

## 📊 Example CRM

| Date       | Name  | Requirement         | Budget  | Status |
| ---------- | ----- | ------------------- | ------- | ------ |
| 09/08/2026 | Rahul | Website Development | ₹50,000 | New    |
| 09/08/2026 | Priya | AI Chatbot          | ₹30,000 | New    |

## ⚙️ Setup

### 1. Install / Open n8n

Create an n8n account or run n8n locally.

### 2. Create Telegram Bot

Create a Telegram bot using BotFather and connect the Telegram credentials in n8n.

### 3. Create Google Sheet

Create a Google Sheet with columns:

```text
Date
Name
Requirement
Budget
Status
```

### 4. Import Workflow

Import the JSON workflow into n8n.

### 5. Configure Credentials

Connect:

* Telegram API
* Google Sheets OAuth

### 6. Activate Workflow

Activate the workflow and send a test message to the Telegram bot.

## 🔐 Security

Before publishing this workflow publicly:

* Remove Telegram credentials.
* Remove Google Sheets IDs.
* Remove private webhook IDs.
* Never upload API keys or access tokens.
* Use environment variables or n8n credentials for sensitive information.

## 🎯 Use Cases

This automation can be used by:

* Freelancers
* Agencies
* Small businesses
* Sales teams
* Marketing teams
* Service providers
* Startups

## 🔮 Future Improvements

Possible improvements include:

* AI-powered lead qualification
* Lead scoring
* Email notifications
* Slack notifications
* Automatic follow-up messages
* CRM integration
* PostgreSQL database
* WhatsApp integration
* Dashboard for lead analytics
* Automatic sales team assignment
* Duplicate lead detection

## 📸 Screenshots

Add screenshots of:

1. n8n workflow
2. Telegram conversation
3. Google Sheets CRM

## 👨‍💻 Author

**Kaushal Kumar**

B.Tech CSE – Artificial Intelligence & Machine Learning

### Skills Demonstrated

`n8n` `Automation` `Python` `JavaScript` `AI` `Telegram API` `Google Sheets` `Data Analytics` `Workflow Automation`

---

⭐ If you find this project useful, consider giving it a star!
