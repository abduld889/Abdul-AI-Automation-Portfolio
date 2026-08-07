### Project Overview
This project automates the process of monitoring a Google Sheet,
processing the collected data with an AI model, and sending the
generated output through Gmail. it demonstrates how AI can be
integrated into business workflows using n8n.
### Workflow Process
#### 1. Google Sheets Trigger
This node monitors the selected google sheet. Whenever a new row is
added or an existing row is updated, it automatically starts the workflow.
#### 2. Aggregate
The Aggregate node collects and organizes the incoming data into a 
structured format before  passing it to the AI model. This ensures 
the information is processed consistently.
#### 3. Basic LLM Chain
This node sends the prepared data to the language model and manages the
interaction between the workflow and AI.
#### 4. Ollama Chat Model
Ollama processes the request and generates an AI response based on the 
instructions defined in the workflow.
#### 5. Gmail
The Gmail node automatically sends the AI-generated response to the specific 
email address.
### Technologies Used:
n8n : Workflow automation platform used to build the entire automation.
Google Sheets Trigger : Detects, changes in the spreadsheet and start the workflow.
Aggregate : Organizes and prepares the data before AI processing.
Basic LLM Chain : Connects the workflow to the AI model.
Ollama Chat Model : Generates the AI response.
Gmail : Delivers the generated response by email.
