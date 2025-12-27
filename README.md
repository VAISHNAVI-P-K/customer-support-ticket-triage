# customer-support-ticket-triage
 Week-1 Internship Project
 
# Workflow Overview

1. Dataset Loading & Exploration

   ▪︎ Loaded CSV dataset in Google Colab
   
   ▪︎ Analyzed rows, columns, missing values, and sample tickets

2. Text Cleaning
 
   ▪︎ Converted ticket descriptions to lowercase
   
   ▪︎ Removed special characters and extra spaces

3. Issue Classification (Rule-Based)
 
   Tickets are classified into the following categories using keyword logic:

   • PAYMENT

   • LOGIN

   • DELIVERY

   • REFUND

   • BUG

   • GENERAL

4. Priority Assignment
 
   Ticket priority is assigned based on message severity:
 
   • P0 – Critical
   
   • P1 – High
   
   • P2 – Medium
   
   • P3 – Low

5. SLA Calculation
   
   ▪︎ Mapped priority levels to SLA hours
   
   ▪︎ Calculated ticket due time using date and time operations

6. Report Generation
   
   ▪︎ Generated a structured support manager report
   
   ▪︎ Exported the final processed dataset as a CSV file

# Dataset

   The dataset contains customer support ticket details including:

   ▪︎ Ticket information

   ▪︎ Customer details

   ▪︎ Ticket subject and description

   ▪︎ Response and resolution timestamps

   The Ticket Description column is used as the primary text input for classification and prioritization.

# Tools and Technologies Used

   ▪︎ Python
   
   ▪︎ Google Colab
   
   ▪︎ Pandas – Data analysis and manipulation
   
   ▪︎ Regular Expressions (re) – Text preprocessing
   
   ▪︎ Datetime Module – SLA and due time calculations
   
   ▪︎ GitHub – Version control and project submission

# OUTPUT 

▪︎ Cleaned and enriched ticket dataset

▪︎ New columns generated:

   - clean_message
   
   - issue_type
   
   - calculated_priority
   
   - sla_hours
   
   - due_time

▪︎ Final output file:

   - final_support_tickets.csv

# Conclusion
 
This project demonstrates how rule-based logic and structured data processing can be used to automate customer support ticket triaging. It reflects real-world engineering practices and serves as a strong foundation for future enhancements such as machine learning-based classification or dashboard visualization.
