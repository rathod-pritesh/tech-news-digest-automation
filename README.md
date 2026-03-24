# 🗞️ Tech News Digest Automation

An automated workflow built with **n8n** that collects the latest tech news from multiple sources, processes it, and sends a clean email digest daily.

---

## 🚀 Features

* ⏰ **Daily automation** using cron schedule (runs every morning)
* 🌐 Fetches latest news from multiple topics:

  * Golang
  * SvelteKit
  * Artificial Intelligence
  * Machine Learning
  * Tech Trends
  * New Technology & Inventions
* 🧹 Filters and removes invalid articles
* 📰 Selects top headlines from each category
* 📧 Sends a structured HTML email digest
* ⚡ Fully automated workflow

---

## 🛠️ Tech Stack

* **n8n** – Workflow automation
* **NewsAPI** – News data source
* **Gmail Node** – Email delivery
* **JavaScript (Code Node)** – Data processing & HTML generation

---

## 📊 Workflow Overview

1. Schedule Trigger runs daily at 9 AM
2. Fetch news from different categories via HTTP requests
3. Merge all responses into a single flow
4. Process articles using JavaScript:

   * Filter invalid entries
   * Select top articles
   * Generate HTML email
5. Check if articles exist
6. Send email digest

---

## ⚙️ Setup Instructions

### 1. Import Workflow

* Download the workflow JSON
* Import into your n8n instance

---

### 2. Configure Credentials

#### 🔐 NewsAPI

* Create **HTTP Header Auth**
* Add:

  * Header: `Authorization`
  * Value: `YOUR_NEWS_API_KEY`

---

#### 📧 Gmail

* Connect your Gmail account
* Select it in the email node

---

### 3. Update Email

Replace:

```txt id="8id4cs"
YOUR_EMAIL_ID
```

with your actual email address.

---

### 4. Activate Workflow

* Turn ON the workflow
* It will run automatically every day

---

## ✨ Output

You receive a daily email containing:

* Top tech headlines
* Short descriptions
* Source and date
* Clean, readable format

---

## 📌 Use Cases

* Stay updated with tech news
* Developer daily digest
* Automated productivity workflows

---
