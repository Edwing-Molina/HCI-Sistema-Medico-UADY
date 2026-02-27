## Requirements Specification - UADY Medical Service App

This document outlines the functional and non-functional requirements for the application dedicated to the beneficiaries of the Medical Service at the Autonomous University of Yucatan.

### 1. Functional Requirements (FR)

| ID | Requirement Name | Description |
| :--- | :--- | :--- |
| **FR01** | **Splash Screen** | The system must display a startup screen with institutional colors and the app version for a minimum of 1.5 seconds as a visual loading indicator. |
| **FR02** | **Office 365 Authentication** | The system must allow login using an institutional Office 365 account via a dedicated button. |
| **FR03** | **Employment Status Validation** | Upon login, the system must verify in real-time if the employee is active in the database; otherwise, display: "User is not active." |
| **FR04** | **Local Data Persistence** | The system must store the access token, full name, email, and employee ID in local storage to prevent redundant queries. |
| **FR05** | **Secure Logout** | The app must invalidate Office 365 and local API tokens, presenting a confirmation modal before proceeding. |
| **FR06** | **Patient Selection** | The system must allow choosing between the employee or their beneficiaries via a mandatory selector that updates the interface dynamically. |
| **FR07** | **Appointment Scheduling** | Users can select specialty, shift, date, and doctor. The calendar will only be enabled after selecting the specialty and shift. |
| **FR08** | **Campus-based Availability** | The system must filter available doctors and schedules based on the employee's assigned campus (e.g., Exact Sciences, Social Sciences). |
| **FR09** | **List and Detail View** | Display future appointments in ascending chronological order with full details: folio, doctor, specialty, shift, date, and time (24h format). |
| **FR10** | **Appointment Cancellation** | Allow cancelling appointments from the list/detail view with a modal warning: "This cancellation counts toward your annual limit." |
| **FR11** | **Cancellation Limit Control** | The system must automatically block scheduling when the configurable limit is reached (default is 3 cancellations). |
| **FR12** | **Administrative Block Notification** | If the user is blocked, display a persistent message indicating that unblocking can only be done via email. |
| **FR13** | **Connection Error Feedback** | Detect lack of internet or timeout (10 sec) and show the message: "We cannot connect to the internet, please check your connection." |
| **FR14** | **Persistent Navigation Menu** | Include a fixed Bottom Navigation Bar with access to Home, Passes, Medical Record, and Appointments. |
| **FR15** | **Beneficiary Search** | Real-time filter starting at 3 characters, case-insensitive and ignoring accents to reduce typing effort. |
| **FR16** | **Settings Screen** | Display the logged-in user's email and provide external links to the Privacy Notice and Operations Manual. |

---

### 2. Non-Functional Requirements (NFR) - Usability & Accessibility

These requirements are designed to mitigate technological barriers for **Manual Labor Users** and visual fatigue for **Faculty/Administrative Staff (ages 45-55)**.

| ID | Attribute | Specification |
| :--- | :--- | :--- |
| **NFR-U-01** | **Legibility** | The interface must support OS font scaling, maintaining a base size of **16px** to ensure readability for the 45-70 age group. |
| **NFR-U-02** | **Contrast** | The design must comply with **AA (WCAG 2.1)** standards with a minimum 4.5:1 contrast ratio to reduce visual fatigue. |
| **NFR-U-03** | **Interactivity** | Buttons and clickable elements must have a minimum target area of **44x44 dp** to facilitate interaction for users with less digital experience. |
| **NFR-U-04** | **Cognitive Load** | The scheduling flow must use progressive disclosure, showing a maximum of 3 fields per screen to avoid overwhelming the user. |
| **NFR-U-05** | **Clear Navigation** | Bottom menu icons (FR14) must include mandatory text labels to ensure the interface does not require advanced organizational skills. |
| **NFR-U-06** | **Human Language** | Errors must be described in natural, non-technical language, always explaining the next step to resolve the issue. |
| **NFR-U-07** | **Visual Feedback** | For any action lasting longer than 200ms, the system must show a loading indicator to mitigate anxiety when using digital interfaces. |