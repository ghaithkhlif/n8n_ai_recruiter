Automated AI Recruitment Agent (n8n + Mistral AI)
This project is a comprehensive n8n workflow designed to automate the screening and analysis of job applications. It leverages Artificial Intelligence to compare incoming resumes against a specific job description and logs the analysis into a tracking spreadsheet.

How It Works
Triggers: The workflow monitors a Gmail inbox (for attachments) and a Google Drive folder.

Context: It automatically retrieves a reference Job Description from Google Drive.

Extraction: Text is extracted from PDF files (both Resumes and Job Descriptions).

AI Analysis: The Mistral AI model compares the candidate's skills against the job requirements.

Parsing: A Structured Output Parser converts the AI response into clean data (Name, Score, Verdict).

Storage: Results are appended to a Google Sheets document for immediate HR review.

Tech Stack
n8n (Self-hosted / Localhost)

Mistral AI (LLM model for screening)

Google Workspace (Gmail, Drive, Sheets)

Setup Instructions
Import the provided .json file into your n8n instance.

Set up your credentials for Google Cloud Console (OAuth2) and Mistral Cloud.

Update the "Job Description" node with your specific File ID.

Create a Google Sheet with the following headers: Name, Score, Strengths, Weaknesses, Verdict.
