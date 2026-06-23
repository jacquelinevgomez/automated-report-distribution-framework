# Automated Reporting Workflow

## Overview

This project automates operational reporting by transforming raw table-based exports into standardized, analysis-ready outputs using Microsoft OneDrive, Power Automate, and Excel Office Scripts.

The solution reduces manual reporting effort, improves consistency across outputs, and enables non-technical users to generate structured reports through a simple file-based workflow.

---

## Workflow

The automation process follows these steps:

1. A report is exported from an operational reporting system  
2. The file is placed into the `Source_Data` folder in OneDrive (manual upload or integrated process)  
3. File placement triggers a Power Automate workflow  
4. An Excel Office Script is executed to transform the raw data  
5. The processed file is saved into the `Final_Outputs` folder  
6. The final file is renamed and distributed to stakeholders  

> Note: The ingestion method is flexible and can be adapted depending on organizational tools (manual upload, scheduled exports, or system integration).

---

## Business Impact

- Reduced manual effort required for report formatting and transformation  
- Standardized reporting outputs across teams  
- Enabled non-technical users to generate consistent reports without advanced Excel knowledge  
- Improved speed of stakeholder reporting delivery  
- Reduced errors caused by manual data manipulation  
- Increased operational efficiency through automation of repetitive tasks  

---

## Technologies Used

- Microsoft OneDrive  
- Microsoft Power Automate  
- Excel Office Scripts (TypeScript)  
- Microsoft Excel  

---

## Features

- Automated detection of new files via OneDrive folder monitoring  
- Trigger-based workflow using Power Automate  
- Office Script-based data transformation  
- Standardized formatting for dashboard-ready outputs  
- Separation of raw data and final outputs for scalability  
- Flexible data ingestion methods (manual or system-driven)  
- Automated file renaming and stakeholder distribution  
- Reusable transformation logic across multiple reports  

---

## Architecture

The workflow follows a simple layered structure:

**Data Inputs → Processing Layer → Output Layer**

- **Data Inputs:** Raw system exports stored in OneDrive  
- **Processing Layer:** Excel Office Scripts for transformation logic  
- **Output Layer:** Cleaned and standardized reports for distribution  

This structure ensures scalability, maintainability, and consistency across multiple reporting workflows.

---

## Screenshots

Add screenshots here to demonstrate:

- Power Automate workflow design  
- OneDrive folder structure  
- Before vs after transformation output  
- Office Script logic (optional snippet or overview)  

---

## Key Design Considerations

- Built to reduce reliance on advanced Excel knowledge  
- Designed for accessibility by non-technical users  
- Focused on standardization and repeatability  
- Adaptable to different data ingestion methods depending on environment constraints  
