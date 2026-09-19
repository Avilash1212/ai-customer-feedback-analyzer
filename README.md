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

The workflow consists of multiple stages that automate the complete feedback-processing pipeline.

```text
CSV Upload
    ↓
Parse CSV
    ↓
Extract Feedback
    ↓
Analyze Feedback
    │
    └── OpenAI Chat Model
    ↓
Prepare Row
    ↓
Write Results to Google Sheets
    ↓
Build Excel File
    ↓
Email Results '''

