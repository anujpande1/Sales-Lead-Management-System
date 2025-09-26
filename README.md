# Salesforce Sales Lead Management System

## Introduction

This project is a comprehensive B2C Salesforce CRM implementation designed to solve common challenges in sales lead management. The system automates the entire lead lifecycle, from initial capture on a website to final reporting on sales performance.  It provides a streamlined process for sales agents and gives management real-time visibility into the sales pipeline through customized reports and dashboards.

This project was built following a structured 10-phase implementation plan, covering everything from initial analysis to final UI configuration.

## Key Features

-   **Automated Lead Capture**: A web-to-lead form to capture inquiries directly from a website, eliminating manual data entry.
-   **Automated Lead Assignment**: A record-triggered Flow that automatically assigns incoming leads to the correct sales representative based on business criteria.
-   **Lead Qualification & Conversion**: A standardized process for qualifying leads and converting them into Accounts, Contacts, and Opportunities.
-   **Opportunity Pipeline Tracking**: Management of deals through a structured sales pipeline using Opportunity stages.
-   **Sales Performance Dashboard**: A centralized dashboard that provides a visual overview of key metrics, including leads by source, the sales pipeline by stage, and lead conversion rates.
-   **Custom Lightning App**: A dedicated "Sales Lead Management" app that provides users with a focused workspace containing only the necessary tabs and features.

## Salesforce Concepts Implemented

This project demonstrates proficiency in a wide range of Salesforce declarative development and administration skills.

* **Automation**
    * **Flow Builder**: Used to create a record-triggered flow for automating lead assignment.
    * **Web-to-Lead**: Standard feature for web form integration.

* **Data Modeling**
    * **Standard Objects**: Utilized Lead, Account, Contact, and Opportunity objects.
    * **Custom Fields**: Added custom fields to standard objects to capture additional data (e.g., `Lead Score`).
    * **Page Layouts**: Customized page layouts for a user-friendly experience.

* **Reporting & Analytics**
    * **Reports**: Created Tabular and Summary reports to analyze data.
    * **Report Charts**: Added charts to reports for better visualization.
    *  **Dashboards**: Built a dashboard with multiple components (Funnel, Bar, Donut charts) for at-a-glance insights[cite: 109].

* **User Interface & Experience**
    *  **Lightning App Builder**: Created a custom Lightning App for a tailored user experience[cite: 69].
    *  **Custom Tabs & Navigation**: Configured app navigation to include relevant tabs[cite: 71].

* **Security & Sharing**
    *  **User Setup**: Created and managed user records[cite: 17].
    *  **Profiles**: Assigned standard profiles to users to control object and field access[cite: 18].
    *  **Roles & Role Hierarchy**: Established a role hierarchy to ensure managers have visibility into their team's data[cite: 19].

## Setup & Configuration Steps

To replicate this project in a Salesforce Developer Org, follow these key steps:

1.   **Org Setup**: Configure basic company settings, create two new users (e.g., a Sales Rep and a Sales Manager), and establish a simple two-level role hierarchy.
2.   **Data Model Customization**: Add a custom picklist field named `Lead Score` to the Lead object and adjust the page layout.
3.  **Automation**:
    * Enable Web-to-Lead and generate the HTML form.
    * Create a record-triggered flow on the Lead object that assigns new leads from the web to your Sales Rep user.
4.  **Reports & Dashboard**:
    * Create three reports: `Leads by Source`, `Sales Pipeline by Stage`, and `Lead Conversion Rate`.
    * Create a `Sales Performance` dashboard and add the three reports as components.
5.  **Create Lightning App**: Use the App Manager to build a new Lightning App named "Sales Lead Management", adding the Home, Leads, Opportunities, Reports, and Dashboards tabs. Assign it to the relevant user profiles.
