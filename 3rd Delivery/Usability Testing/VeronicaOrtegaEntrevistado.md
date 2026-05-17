# Software Quality and Usability Evaluation - Verónica Ortega

## I. Module: Login

### 1. Attribute: Error Protection

### Scenario: Email Format Validation

- **Errors:** 0 attempts (The user typed her institutional email address with the correct format on her first try).
- **Message Comprehension:** Not applicable (The email format error message was not triggered).
- **Recovery:** 0 (Did not require fixing the email address string format).

### Scenario: Credential Error Feedback

- **Errors:** 1 failed attempt (The user experienced authentication issues during her first attempt due to an initial confusion with her password characters or the Microsoft federated login portal, requiring a second attempt).
- **Message Comprehension:** Yes (She understood that the initial block was due to incorrect entry data).
- **Recovery:** 1 (She re-entered her credentials autonomously until achieving successful validation).

### Scenario: Empty Field Submission

- **Errors:** 0 attempts (The user did not try to click the login button with blank fields).
- **Message Comprehension:** Not applicable.
- **Recovery:** Not applicable.

### 2. Attribute: Accessibility

### Scenario: Interface Scaling for Older Adults

- **Visibility:** The user does not have operating system text scaling active but prefers text to be as large as possible. She had to focus extra visual attention to validate the small font characters after the initial login failure.
- **Layout Integrity:** The login interface elements maintained their standard alignment and proportion on the device screen.

### Scenario: Color-Independent Error Messages

- **Message Comprehension:** Yes (She identified the initial authentication denial through the system's text alerts without relying on color codes).
- **Visibility:** Understood the visual text notice as a security warning.

### Scenario: Keyboard Navigation

- **Task Completion:** The user successfully completed the login process by operating the virtual on-screen keyboard to fix her password and clicking the main access button.
- **Errors:** 1 stumble (Typing/character capturing error during her first password entry).
- **Efficiency:** Processing time was prolonged due to the need to delete, rewrite, and validate the input credentials.

### 3. Attribute: Learnability

### Scenario: Login Flow Recognition

- **Task Completion:** Yes, the user identified the Microsoft institutional login button, although she made an exploratory clarification question to the evaluator prior to clicking.
- **Efficiency:** Moderate due to the initial recognition pause and the subsequent credential re-attempt.
- **Errors:** 0 clicks on incorrect menus or components prior to hitting the login trigger.

### Scenario: Login Loading State Visibility

- **Errors:** 0 (She patiently waited for the system to process the asynchronous authentication without clicking the button repeatedly while loading).
- **Awareness:** Yes, she recognized the system processing states between the first failed attempt and the final dashboard access.

### Scenario: Password Correction

- **Errors:** 1 correction (She had to clear and completely retype her password after the initial login failure).
- **Completion:** Yes, she managed to complete the login task successfully on her second attempt.
- **User Reaction:** Displayed focused concentration and a slight pause to guarantee the accurate entry of her account data.

### 4. Attribute: Satisfaction

### Scenario: Session Persistence

- **Task Completion:** Yes, after completing the background application force-close (Task 2), the system kept the session token active and loaded the Dashboard immediately upon reopening.
- **User Reaction:** The user assimilated the persistence behavior and moved directly to the next steps without showing confusion about not needing to re-login.

### Scenario: Interface Trust and Professional Appearance

- **Perceived Trust:** High (Using the integrated institutional login view conveys security to the user, who marked it in her profile as the easiest and most secure method).
- **Message Comprehension:** Yes, she clearly understood that this screen represented the official gateway to the university's medical record system.

---

## II. Module: Appointments

### 1. Attribute: Accessibility

### Scenario: Motor Precision and Fatigue

- **Errors:** 0 accidental clicks outside targets or on adjacent form selectors.
- **Task Completion:** Yes, she selected all parameters from the dropdown menus with high precision and physical ease.
- **Visibility:** No coordination issues or physical fatigue were observed when interacting with the form elements.

### Scenario: Visual Readability (Presbyopia)

- **Message Comprehension:** Not applicable (The cancellation threshold banner was not triggered since the user completed the happy path seamlessly).
- **Visibility:** Did not require bringing the device unusually close to her face to interpret the readable appointment text strings.

### Scenario: Outdoor Contrast and Visibility

- **Visibility:** Not applicable (The test was performed indoors under stable and controlled lighting conditions).
- **Message Comprehension:** Validated the status of her requests within the main list accurately.
- **Questions asked:** None regarding contrast or background readability.

### Scenario: Backwards Navigation (Cognitive)

- **Awareness:** Yes, the user effectively identified and used the structural navigation controls to go back and check her active appointment list status.
- **Abandonment Rate:** 0% (Remained active and engaged throughout the workflow).
- **Questions asked:** None.

### Scenario: Logical Reading Order (Assisted/Cognitive)

- **Message Comprehension:** Yes, she interpreted and validated the structured appointment card information on the screen correctly.
- **Questions asked:** Zero doubts about schedules, dates, or assigned doctors.
- **Flow block:** 0 cognitive blocks.

### 2. Attribute: Learnability

### Scenario: Intuitive Navigation (Discovery)

- **Errors:** 0 (She immediately located the golden "Book an appointment now" button from the main screen without drifting into other app sections).
- **Questions:** 0 disorientation questions inside the user interface.
- **Task Efficiency:** Direct and immediate entry to the scheduling transaction flow.

### Scenario: Clear Form Flow

- **Click Count:** Completed the field parameters using the exact steps established by the interface architecture design.
- **Drop-off Rate:** 0% (Successfully finalized the data entry for the appointments).

### Scenario: Recognition of Primary Action (Action Button)

- **Visibility:** Yes, the visual layout hierarchy allowed her to immediately identify the primary button as the core action trigger.
- **Questions:** 0 questions regarding how to initiate a new request.
- **Errors:** 0 clicks on static or dead target layout areas.

### Scenario: Learning "Progressive Disclosure"

- **Flow block:** 0 blocks (She easily understood the top-to-bottom dependency where selecting a date and specialty conditionally unlocks available time slots and physicians).
- **Comprehension:** Filled out the form fields sequentially and logically without skips.
- **Efficiency:** Continuous forward progress across conditional selectors.

### Scenario: Use of Date Selector (Digital Calendar)

- **Errors:** 0 blocks or lockups navigating the component within the active working range of the current month (May).
- **Questions:** 0 doubts concerning calendar navigation UI logic.
- **Completion:** Yes, set the requested dates straightforwardly.

### Scenario: Specific Doctor Search

- **Visibility:** Yes, she identified the picker selector to find and swap the assigned physician from the pool.
- **Click Count:** 2 clicks (1 to open the doctor picker dropdown list and 1 to confirm the chosen name).
- **Errors:** 0 misclicks on contiguous text rows.
- **Questions:** 0 questions about altering the assigned healthcare provider.
- **Recovery:** Fluid and effective selection of Dr. Herrera.

### 3. Attribute: Error Protection

### Scenario: Recovery from "No Results"

- **Recovery:** Upon returning to the main list and noticing the app layout didn't refresh instantly, the user manually flipped between tab bars to force a UI synchronization and refresh the dashboard autonomously.
- **Comprehension:** Evaluated and understood the mild network rendering latency.

### Scenario: Confirmation of Irreversible Action

- **Errors:** 0 accidental cancellations (All performed cancellations explicitly matched the evaluation test steps).
- **Recovery:** Yes, she interacted seamlessly with the modal confirmation prompt box in a clear and assertive manner.

### Scenario: Prevention of Past Appointments

- **Errors:** During Task 5, when attempting to choose a past month (April), the built-in calendar rules blocked retrogressive selections. The user recognized this lock and verbally stated, "It says it's not allowed."
- **Questions:** 0 questions; she immediately absorbed the passive visual calendar constraints.
- **Recovery:** Safely moved past the action independently, respecting the application's underlying business rules.

### 4. Attribute: Satisfaction

### Scenario: Sense of Achievement

- **Completion:** Completed successfully. Unlike other participants, this user had no registered family dependents active on her profile record ("Has family members registered as beneficiaries: No"). Thus, she executed the test cancellations directly upon her own primary account flow, concluding the evaluation smoothly.
- **Questions:** 0 queries regarding the final system status.
- **Comprehension:** Correctly identified the updated appointment status and verified the transaction endpoint inside the user interface.

---

## Usability Metrics Table per Task

| Module           | Task                                                   | Completed? (Yes/No) | No. of Clicks | No. of Questions | No. of Errors / Stumbles |
| :--------------- | :----------------------------------------------------- | :-----------------: | :-----------: | :--------------: | :----------------------: |
| **Login**        | **Task 1:** Log in using account credentials           |         Yes         |       5       |        1         |            1             |
| **Login**        | **Task 2:** Restart application (Verify persistence)   |         Yes         |       2       |        0         |            0             |
| **Appointments** | **Task 1:** Book a primary medical appointment         |         Yes         |       7       |        0         |            0             |
| **Appointments** | **Task 2:** Verify success status in main list         |         Yes         |       1       |        0         |            0             |
| **Appointments** | **Task 3:** View basic data elements on card summary   |         Yes         |       0       |        0         |            0             |
| **Appointments** | **Task 4:** View full detailed info of the appointment |         Yes         |       1       |        0         |            0             |
| **Appointments** | **Task 5:** Attempt to book in a past month (April)    |         Yes         |       3       |        0         |            1             |
| **Appointments** | **Task 6:** Book an appointment for a dependent        |         Yes         |       0       |        0         |            0             |
| **Appointments** | **Task 7:** Cancel active medical appointments         |         Yes         |       3       |        0         |            0             |
