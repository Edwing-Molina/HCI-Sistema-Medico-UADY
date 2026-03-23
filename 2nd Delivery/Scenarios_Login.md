# Usability Scenarios – Login Module

To provide a solid technical foundation for the project, We build scenarios with the metrics defined in **MétricasHCI.pdf** with the synthetic personas.
Integrating the scenarios with these metrics, **clear acceptance parameters** are established to determine when the system reach the expected usability and quality standards.

These scenarios are specifically designed to evaluate the usability attributes of the **Login Module**.

---

# Detailed Usability Scenarios

## Scenario 1: Don José’s Inclusive Access

This scenario evaluates the system’s ability to **avoid excluding users with technological barriers** and its capability for **effective error recovery**.

| Element       | Scenario Details                                                                                                                                                                                                                                      | Control Metric (MétricasHCI.pdf)                                           |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| **Persona**   | **Don José** (Maintenance staff member).                                                                                                                                                                                                              | **Attribute:** Learnability                                                |
| **Context**   | He is in the UADY maintenance workshop during a break. He attempts to sign in using Office 365 but fails because he cannot remember his institutional password.                                                                                       | **Attribute:** Error Handling                                              |
| **Task**      | Locate and use the **alternative login method** (Employee ID or CURP) to access the application for the first time.                                                                                                                                   | **Goal:** Complete the task in **less than 3 minutes** without assistance. |
| **Narrative** | Don José opens the application. After the institutional login fails, the system displays a clear message in plain language explaining the next step. He finds the alternative login button, enters his information, and the system grants him access. | **Goal:** Error recovery success rate greater than **90%**                 |
| **Outcome**   | Don José successfully accesses the system and feels confident about using the application in the future.                                                                                                                                              | **Metric:** Average execution time for the first task                      |

---

## Scenario 2: Dr. Elena’s Visual Efficiency

This scenario validates that the interface design **does not cause visual fatigue** and that the system provides **clear and timely feedback** to the user.

| Element       | Scenario Details                                                                                                                                                                                                                                                      | Control Metric (MétricasHCI.pdf)                           |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| **Persona**   | **Dr. Elena** (Senior academic staff member).                                                                                                                                                                                                                         | **Attribute:** Visual Accessibility                        |
| **Context**   | At the end of her workday. She experiences visual fatigue and uses the application from her office under artificial lighting conditions.                                                                                                                              | **Attribute:** System Status Visibility (Feedback)         |
| **Task**      | Perform a quick login using Office 365 to verify a medical pass.                                                                                                                                                                                                      | **Attribute:** Cognitive Load Reduction                    |
| **Narrative** | Dr. Elena opens the application. Thanks to the proper visual contrast (4.5:1) and a minimum font size of 16px, she can easily identify the login button. After pressing "Sign In", a loading indicator appears, confirming that the system is processing the request. | **Goal:** Visual response time less than **5 seconds**     |
| **Outcome**   | Dr. Elena accesses the system within a few seconds without experiencing technological anxiety or visual strain.                                                                                                                                                       | **Goal:** Score higher than **80 points** on the SUS scale |
