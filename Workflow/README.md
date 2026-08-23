### Overview
This project is an automated customer order processing workflow built
with n8n. it receives customer order information through a webhook, 
organizes the incoming data, records the order in Google sheets, applies
conditional logic, and sends automated notifications through an HTTP API
and Gmail.
#### Workflow
## Webhook > Edit Fields > Google Sheets > IF > HTTP Request > Gmail
Webhook : Receives the customer's order information through a POST request.
Edit Feilds : Processes and organizes the incoming customer data into the 
required fields for the next steps.
Google Sheets : Appends or updates the customer's order information in a 
Google Sheets spreadsheet, creating a centralized record of orders.
IF Node : Uses conditional logic to determine wether the order should continue
to the next stage of the automation.
HTTP Request : Sends the required order information to an external API using 
HTTP POST request. In this workflow, the AOI integration is used for automated
customer communication.
Gmail : Sends an automated email notification after the order reaches the final
stage of the workflow.
#### Technologies Used
1. n8n : workflow automation
2. Webhook : Rceiving Customer Orders
3. Google Sheets : Order data storage
4. HTTP Request/Rest API : External service integration
5. Gmail : Automated email notification 
6. JSON : Workflow configuration and portability
#### Purpose
This prroject demonstrates practical skills in workflow automation, API integration,
data management, conditional logic, and automation communication.
