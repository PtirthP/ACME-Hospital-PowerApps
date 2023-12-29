# ACME Hospital Out of Network Notification Project

## 🚨 Note: Source Code Only 🚨

**Please be aware that the files available in this GitHub repository contain the source code for the application only. Automated flows for tasks such as retrieving CSV, sending emails, and notifications are not included. This repository is specifically for the application's source code.**


## Project Overview

ACME Hospital Out of Network Notification Project is a comprehensive solution designed to address compliance with the “Cures Act” Information Blocking Rule. Leveraging Microsoft Power Platform, the application ensures efficient patient data management, real-time notifications, and seamless integration with Microsoft services.

## Key Components

### Infrastructure

The project relies on Microsoft Power Platform, a cloud-based service offering scalability and reliability. Key components include:
- **Scalability:** Cloud-based infrastructure, model-driven architecture, and integration capabilities facilitate scalability.
- **Reliability:** Global data centers of Microsoft ensure high availability and low latency, guaranteeing consistent performance.

### Architecture

Deeply rooted in Microsoft Power Platform, the architecture highlights:
- **PowerApps:** The application utilizes PowerApps, fetching data from a SharePoint list for benefits in data consistency and seamless integration with other Microsoft services.
- **Integration:** PowerApps seamlessly connects with services like SharePoint and Power Automate, ensuring efficient data flow between components.
- **Data Flow:** A well-defined path from CSV data source through Power Automate to SharePoint entries, demonstrating efficient and structured data management.

### Security

Azure contributes significantly to data security:
- **Data Security:** Encryption protocols for data in transit and at rest, multi-layered security, and continuous monitoring protect patient information.
- **Compliance:** Adherence to industry standards like GDPR and HIPAA ensures regulatory compliance.

## Technical Details

### Database Design DFD

- **Entities:** Health Information Exchange, ACME Hospital (SFTP), Power Automate, Power Apps, Physicians.
- **Datastores:** CSV File, SharePoint List.
- **Processes:** Sending CSV to ACME SFTP, Storing CSV, Power Automate Conversion Flow, Power Automate Notification Flow, etc.
- **Data Flow:** ACME hospital receives CSV from HIE, Power Automate converts and notifies PowerApps, Physicians access patient information.

### Working Prototype Storyboard/Wireframe - UX/UI/HCI Design

- **Login Page:** User authentication and password recovery.
- **Authentication Screen with MFA:** Multi-Factor Authentication for enhanced security.
- **Home Page:** Navigation to patient list, notifications, and search functionalities.
- **Notifications:** Real-time alerts for physicians about patient visits.
- **Patient List and Details:** Access to patient information with editing and note-taking features.


## Quality Planning, Quality Assurance, Quality Control

### STLC Plan

| STLC Stage         | Entry Criteria                                             | Activity                                                                                                    | Exit Criteria                                                                                              | Deliverables                                                                                                                                    |
|--------------------|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| Requirement Analysis| - Approved project initiation                             | - Defined project scope and constraints.<br> - Identified key stakeholders.                                  | - A comprehensive understanding of project requirements.<br> - A detailed scope and constraints.<br> - Risk assessment report, highlighting potential testing challenges | - Project Feasibility.<br> - Project Charter.<br> - Project Schedule with Time Management.<br> - Use Cases with Diagrams for PowerApps Application. |
| Test Planning       | - Approved requirement analysis                           | - Clear project scope<br> - Defined test strategy<br> - Identified test environment needs                    | - A comprehensive test plan outlining objectives, schedules, resources.<br> - Identified test environments and tools.<br> - Test schedule and resource allocation | - Project Technical Design.<br> - Project Security, Infrastructure, Architecture.<br> - Data Flow Diagram detailing all processes within the working application. |
| Test Case Development| - Approved test plan                                       | - Defined test cases and scenarios<br> - Access to test data (patient list)<br> - Identified test environment  | - Test cases and scenarios covering all aspects of the application.<br> - Test data prepared for execution.<br> - Test case specifications and documentation | - Power Automate Flow for incoming CSV file.<br> - Creation of SharePoint List from CSV File.<br> - Power Automate Flow for notifying application users (physicians) of new patients. |
| Test Environment setup| - Defined test environment needs                          | - Availability of the required test environment<br> - Access to PowerApps licenses                           | - Configured test environment<br> - PowerApps licenses activated and available<br> - Documented setup procedures  | - Working PowerApps Application.<br> - Populated patient data implemented into app environment from SharePoint list.<br> - Working patient list updates when changed in PowerApps Application. |
| Test Execution       | - Defined test cases                                       | - Prepared test data (SharePoint List)<br> - Availability of test environment on PowerApps<br> - Access to PowerApps licenses  | - Test execution results<br> - Defective application with bugs<br> - If the application is defective, debug and execute again  | - Working PowerApps Application implementation with no bugs.<br> - Full integration of patient data in the application. |
| Test Cycle closure   | - Completed test execution                                | - All defects resolved and retested<br> - Test environment ending                                           | - Test summary report, including test results, defect summary, and compliance status.<br> - Verified and validated application readiness for deployment.<br> - Lessons learned documentation and recommendations for future projects | - Project Testing Closure Report.<br> - PowerApps Application Release to Users. |

## Activation Plan

### Infrastructure Setup

1. **Dataverse Configuration:** Establish a tailored Dataverse environment.
2. **Security Configuration:** Implement role-based access controls in Dataverse.
3. **Integration with Power Platform:** Ensure seamless interaction between Dataverse and Power Platform.
4. **Modify Power Automate Flows:** Redirect data writing processes to Dataverse.
5. **Scalability Planning:** Evaluate and plan for scalability with Dataverse.

### Readiness Steps

1. **User Training:** Conduct training sessions for end-users.
2. **Documentation and Knowledge Transfer:** Update documentation reflecting changes.
3. **User Acceptance Testing (UAT):** Thorough testing with stakeholders.
4. **Performance Testing:** Verify optimal performance under different scenarios.
5. **Post-Implementation Support Plan:** Develop a comprehensive plan for ongoing support.
6. **Communication and Rollout:** Communicate the transition to Dataverse to all stakeholders.

## Implementation Plan – Rolling out to Medical Staff

1. **Infrastructure Integration:** Integrate Dataverse seamlessly with Power Platform.
2. **Communication Plan:** Define communication channels and notify physicians.
3. **User Acceptance Testing:** Instruct users on the new application and collect feedback.
4. **Monitoring and Feedback:** Continuously monitor application performance and gather user feedback.
5. **Documentation:** Create user manuals and troubleshooting instructions.
6. **Security Measures:** Ensure robust security measures in compliance with HIPAA standards.

## Post Implementation Plan

- **Specialized Support Team:** Establish a support team with defined SLAs.
- **Communication Channels:** Help desk, hotline, email, and support ticket system.
- **Continuous Monitoring:** Implement technologies for performance tracking.
- **Input Collection:** Gather user input through surveys for continuous improvement.
- **Regular Meetings:** Schedule meetings with stakeholders for feedback and planning.
- **Disaster Recovery Plan:** Ensure data backup and drills for data protection.
- **Post-Implementation Report:** Summarize accomplishments, lessons learned, and recommendations.

