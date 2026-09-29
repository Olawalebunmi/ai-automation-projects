AI Task Prioritizer – Make.com + Google Gemini + Airtable

An AI-powered task prioritization automation built with Make.com, Airtable, and Google Gemini.

The workflow monitors new tasks in Airtable, sends the task information to Google Gemini for AI analysis, and updates the Airtable record with the generated priority/assessment.

Technologies Used

- Make.com
- Airtable
- Google Gemini AI
- AI Prompt Engineering
- Workflow Automation

Workflow

Airtable → Google Gemini AI → Airtable

Airtable – Watch Records
The automation monitors Airtable for new or updated task records.

Google Gemini AI – Generate a Response
Gemini analyzes the task information and determines the appropriate priority based on the instructions provided in the prompt.

Airtable – Update a Record
The AI-generated result is written back to the corresponding Airtable record.

Purpose

The goal of this automation is to reduce manual task prioritization and help users quickly identify which tasks require attention.

Architecture Workflow

The AI Task Prioritizer uses Make.com as the automation layer to connect Airtable with Google Gemini AI.

Airtable → Make.com → Google Gemini AI → Make.com → Airtable

1. Airtable – Watch Records
   - Detects a new or updated task.
   - Sends the task information into the automation.

2. Make.com – Automation Layer
   - Receives the Airtable data.
   - Maps the task information into the Gemini prompt.
   - Sends the request to Google Gemini AI.

3. Google Gemini AI – AI Processing
   - Analyzes the task.
   - Determines its priority.
   - Generates the required AI response.

4. Make.com – Data Mapping
   - Receives the Gemini response.
   - Maps the AI output to the appropriate Airtable fields.

5. Airtable – Update Record
   - Writes the AI-generated result back to the original task.


Key Skills Demonstrated

- No-code/low-code automation
- AI workflow integration
- Google Gemini API integration
- Airtable automation
- Data mapping between applications
- Prompt engineering
- Automated record processing
- AI-assisted decision workflows