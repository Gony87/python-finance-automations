# Resumo de Links para Email — n8n Workflow

Automated workflow that reads article links from Google Sheets, 
summarises them using Gemini AI, and sends the summary by email.

## How it works
1. Schedule Trigger — runs automatically
2. Google Sheets — reads links to summarise
3. If — checks if already sent (avoids duplicates)
4. HTTP Request — fetches article content
5. HTML — extracts text from HTML
6. Gemini AI — summarises the article
7. Gmail — sends summary by email
8. Update row — marks as "Resumo ja enviado" in Sheets

## How to use
1. Import `resumo-links-email.json` into your n8n instance
2. Configure Google Sheets, Gmail and Gemini credentials
3. Add links to your Google Sheet
4. Activate the workflow
