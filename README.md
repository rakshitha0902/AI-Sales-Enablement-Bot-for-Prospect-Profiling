🧠 AI-Powered Lead Intelligence Workflow
This project contains a suite of modular n8n workflows that automate the process of scraping, researching, and enriching leads using AI.

🔧 Tools & Stack
n8n for visual workflow automation

SerpAPI for LinkedIn and web scraping

Perplexity AI for contextual lead summarization

Google Sheets for lead storage

Telegram + Webhooks for real-time input/output

📁 Workflow Files
Lead_scraper.json
This workflow collects lead information (locations, industries, job titles) from the user and uses SerpAPI to extract company and profile data. The results are saved to Google Sheets.

Lead_researcher.json
This workflow receives a LinkedIn URL and performs detailed research using:

SerpAPI (to extract structured data)

Perplexity AI (to generate summaries)

Optional company + article lookup

It outputs:

Personal summary

Experience and education

Company profile

Relevant articles

LinkedIn post highlights

Lead_generator.json
An AI agent interface (e.g., Lead Generation Joe) that prompts the user to input data, calls the appropriate scraping or research workflows, and communicates via chat.

📌 Features
✅ End-to-end lead research automation

✅ Modular workflows for scraping and enrichment

✅ HTML-formatted summaries for direct use in CRMs or sales briefings

✅ Works with AI Agents via tools like n8n, Langchain, or Relevance AI

✅ Easily extendable with APIs like Clearbit or Apollo

🚀 How to Use
Clone the repo or download the .json workflows.

Import into your n8n instance.

Configure:

SerpAPI key

Perplexity API key

Google Sheets credentials (for scraping)

Trigger Lead_generator.json from a chat, form, or webhook.

✨ Example Use Case
"Find all CTOs in Berlin working in SaaS startups"
✅ Lead_scraper.json scrapes the leads
✅ Lead_researcher.json enriches them
✅ Result: Fully structured brief per lead, with company context and relevant articles
