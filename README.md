# AI Customer Feedback Analyzer

An AI-powered automation workflow that processes customer feedback from CSV files, analyzes sentiment, structures the results, and automatically delivers the processed insights through Google Sheets, Excel, and email.
## Problem Statement

Organizations collect customer feedback from surveys, support interactions, reviews, and other channels. As the volume of feedback increases, manually reviewing and categorizing each response becomes time-consuming and difficult to scale.

Raw feedback is usually unstructured text, making it harder for teams to quickly identify customer sentiment and turn large volumes of responses into structured information.

This project addresses the problem by automating the initial analysis and processing of customer feedback.

### Objective

The workflow is designed to:

- Accept customer feedback in CSV format
- Extract individual feedback entries
- Analyze feedback using an AI model
- Structure the analysis into rows
- Store the results in Google Sheets
- Generate an Excel report
- Automatically email the processed results
## Solution Overview

This project automates the end-to-end processing of customer feedback using a workflow automation platform and an AI model.

The workflow takes a CSV file containing customer feedback, parses and extracts the feedback entries, sends them to an AI model for analysis, prepares the results in a structured format, and delivers the final output through Google Sheets, Excel, and email.

### Workflow Flow

CSV Upload  
↓  
Parse CSV  
↓  
Extract Feedback  
↓  
AI Feedback Analysis  
↓  
Prepare Structured Results  
↓  
Write Results to Google Sheets  
↓  
Generate Excel File  
↓  
Email Results
## Workflow Architecture

## Workflow Architecture

The workflow is divided into several stages:

1. **CSV Upload**  
   The workflow receives a CSV file containing customer feedback.

2. **Parse CSV**  
   The uploaded CSV file is parsed into individual records.

3. **Extract Feedback**  
   The relevant feedback information is extracted from each record.

4. **Analyze Feedback**  
   Each feedback entry is analyzed using an OpenAI chat model.

5. **Prepare Row**  
   The analysis results are formatted into a structured row.

6. **Write Results to Google Sheets**  
   The processed results are stored in Google Sheets.

7. **Build Excel File**  
   The processed data is converted into an Excel file.

8. **Email Results**  
   The generated results are automatically delivered through email.

   ## Business Impact

The workflow reduces the manual effort required to process and distribute customer feedback.

### Key Business Benefits

- **Reduced manual processing:** Automates CSV parsing, feedback analysis, spreadsheet preparation, Excel generation, and email distribution.
- **Faster feedback review:** Processes batches of feedback automatically instead of requiring manual review of each entry.
- **Consistent first-pass analysis:** Applies the same AI analysis process across feedback entries.
- **Faster stakeholder access:** Results are written to Google Sheets, exported to Excel, and distributed by email without additional manual preparation.
- **Reusable workflow:** The same workflow can be reused for recurring customer feedback-processing tasks.

### Business Use Case

A product or customer experience team can upload a batch of customer feedback and automatically receive structured analysis that can be reviewed and shared with stakeholders.
## Key Features

- **CSV-based feedback ingestion:** Accepts customer feedback in CSV format.
- **AI-powered analysis:** Uses an OpenAI chat model to analyze customer feedback.
- **Structured output:** Converts AI analysis into structured rows for easier processing.
- **Google Sheets integration:** Automatically stores processed feedback in Google Sheets.
- **Excel report generation:** Creates an Excel file containing the processed results.
- **Automated email delivery:** Sends the generated results through email.
- **End-to-end automation:** Connects data ingestion, AI analysis, storage, reporting, and delivery into a single workflow.

## Tech Stack

- **Workflow Automation:** n8n
- **AI Model:** OpenAI Chat Model
- **Data Input:** CSV
- **Data Storage:** Google Sheets
- **Report Generation:** Excel
- **Email Automation:** Email

## Example Input & Output

### Input

The workflow accepts a CSV file containing customer feedback records.

Example:

| Customer | Feedback |
|---|---|
| Customer 1 | The installation process was smooth and the support team was helpful. |
| Customer 2 | The product is useful, but the response time from support could be improved. |
| Customer 3 | I had difficulty getting my issue resolved. |

### Output

The workflow processes the feedback using an AI model and prepares the results in a structured format.

The processed results are then:

- Stored in Google Sheets
- Generated as an Excel file
- Delivered through email
