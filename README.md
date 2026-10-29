# n8n Invoice Parser

This project automates the process of extracting data from invoices and saving it to Google Sheets. It also sends an email with the extracted information in a clean, readable format.

I built this workflow using n8n to make invoice handling easier and reduce the need to enter invoice details manually.

## What it does

- Accepts an invoice through a form.
- Extracts data from the uploaded PDF.
- Uses AI to identify important invoice details.
- Processes the extracted data using JavaScript.
- Adds the invoice details to Google Sheets automatically.
- Formats the information into an email and sends it through Gmail.

## Tools Used

- **n8n** – Workflow automation
- **Qwen Cloud Chat Model** – AI-powered information extraction
- **JavaScript** – Data processing and email formatting
- **Google Sheets** – Store invoice details
- **Gmail** – Send the formatted email
- **PDF extraction** – Read invoice content from uploaded files

## How the Workflow Works

1. Upload an invoice using the form.
2. The workflow extracts the content from the PDF.
3. The AI model identifies the required invoice information.
4. JavaScript processes the extracted data.
5. The invoice details are added to Google Sheets.
6. The workflow prepares a formatted email and sends it through Gmail.

## Setup

To use this workflow on your own n8n instance:

1. Download `invoice_parser.json` from this repository.
2. Open n8n and import the downloaded workflow.
3. Configure the Qwen Cloud Chat Model credentials.
4. Connect your Google Sheets account and select the spreadsheet where invoice data should be stored.
5. Configure your Gmail account and email settings.
6. Test the workflow with an invoice PDF.

You may need to adjust the spreadsheet columns and email settings to match your requirements.

## Testing

I tested the workflow by uploading an invoice PDF. The extracted information was added to Google Sheets, and the email was sent successfully in the expected format.

## What I Learned

While building this project, I worked with AI-based data extraction, PDF processing, JavaScript transformations, Google Sheets integration, Gmail automation, and connecting different services in a single n8n workflow.

## Project File

- `invoice_parser.json` – The exported n8n workflow.

---

**Note:** You need to configure your own credentials before running this workflow. No API keys or account credentials should be shared publicly.
