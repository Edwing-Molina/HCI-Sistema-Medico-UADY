# Software Quality and Usability Evaluation - Elda Sihualpilli Becerra Sierra

# Software Quality and Usability Evaluation - Elda Becerra

## I. Module: Login

### 1. Attribute: Error Protection
### Scenario: Email Format Validation
- **Errors:** 2 attempts (The user entered an invalid email format during the test by mistyping one letter of the email address used).
- **Message Comprehension:** Yes (She understood the invalid format/incorrect email error message on her first attempt).
- **Recovery:** 1 (Required correcting the email format).

### Scenario: Credential Error Feedback
- **Errors:** 1 failed attempt (The user experienced authentication issues during her first attempt due to an initial confusion with her password characters, requiring an additional attempt).
- **Message Comprehension:** Yes (She understood that the initial block was due to the entry of incorrect data).
- **Recovery:** 1 (She re-entered her credentials autonomously until achieving successful validation).

### Scenario: Empty Field Submission
- **Errors:** 0 attempts (The user did not attempt to submit the form with empty fields).
- **Message Comprehension:** Not applicable.
- **Recovery:** Not applicable.

### 2. Attribute: Accessibility
### Scenario: Interface Scaling for Older Adults
- **Visibility:** The user perfectly visualized the text fields and labels in their default size.
- **Layout Integrity:** The elements of the login interface maintained their standard alignment and correct proportions.

### Scenario: Color-Independent Error Messages
- **Message Comprehension:** Yes (She identified the authentication denials without relying on color codes).
- **Visibility:** She understood the visual text notices indicating the initial password errors.

### Scenario: Keyboard Navigation
- **Task Completion:** The user successfully completed the login process by operating the virtual on-screen keyboard to fix her password and clicking the main access button.
- **Errors:** 1 stumble (Typing/character capturing error during her first password entry).
- **Efficiency:** Processing time was prolonged due to the need to delete, rewrite, and validate the input credentials.

### 3. Attribute: Learnability
### Scenario: Login Flow Recognition
- **Task Completion:** Yes, the user located the login button instantly.
- **Efficiency:** Immediate discovery of the primary login action button.
- **Errors:** 0 (Did not click on incorrect elements prior to the login button, although she asked to confirm if that was the correct button).

### Scenario: Login Loading State Visibility
- **Errors:** 0 (Did not tap the button repeatedly while loading).
- **Awareness:** Yes, the user waited patiently for the validation loading process to complete without showing signs of frustration.

### Scenario: Password Correction
- **Errors:** 1 failed attempt (She had difficulty typing her password).
- **Completion:** Yes, but she had to retry entering the password.
- **User Reaction:** Displayed focused concentration and a slight pause to guarantee the accurate entry of her account data.

### 4. Attribute: Satisfaction
### Scenario: Session Persistence
- **Task Completion:** Yes, when fully closing the application and reopening it (Task 2), the system maintained the active session token for the test account and loaded the user profile directly.
- **User Reaction:** The user showed no confusion and proceeded directly into the workflow, assimilating the persistence seamlessly.

### Scenario: Interface Trust and Professional Appearance
- **Perceived Trust:** High (Despite the issue when typing her password, the user perceived the integrated institutional login as a highly secure and trustworthy method).
- **Message Comprehension:** Yes, she fully recognized the screen as the official gateway to the medical system.

---

## II. Module: Appointments

### 1. Attribute: Accessibility
### Scenario: Motor Precision and Fatigue
- **Errors:** 0 accidental clicks on blank areas or adjacent form dropdown selectors during the scheduling process.
- **Task Completion:** Yes, she precisely selected the target parameters (Specialty, Shift, Date, Doctor, and Time slots) and booked the appointment without any physical difficulty. However, while the booking itself was seamless, she experienced friction later when trying to locate the details of the scheduled appointment.
- **Visibility:** No motor fatigue or extreme screen-to-face proximity was observed during this specific step.

### Scenario: Visual Readability (Presbyopia)
- **Message Comprehension:** Not applicable (The cancellation threshold banner was not triggered since the user completed the happy path seamlessly).
- **Visibility:** Did not require bringing the device unusually close to her face to interpret the readable appointment text strings.

### Scenario: Outdoor Contrast and Visibility
- **Visibility:** Not applicable (The evaluation was conducted in an indoor space with stable lighting conditions).
- **Message Comprehension:** She was able to read the interface text perfectly under the current lighting conditions, although the challenge lay in navigating to find the appointment details rather than visually reading them.
- **Questions asked:** None regarding contrast or background visibility.

### Scenario: Backwards Navigation (Cognitive)
- **Awareness:** The user navigated the interface but experienced cognitive friction when trying to find her scheduled appointment information, requiring extra exploratory navigation and tab switching to finally locate where the system stored her active appointment details.
- **Abandonment Rate:** 50% (She delved deep into the system looking for her appointment details and ended up reaching the medical records section, at which point she requested and was provided assistance).
- **Questions asked:** None.

### Scenario: Logical Reading Order (Assisted/Cognitive)
- **Message Comprehension:** Yes, once she successfully located the appointment card, she correctly interpreted the structured appointment data on the screen.
- **Questions asked:** Zero doubts regarding the schedule, doctor, or specialty consulted once the information was on screen.
- **Flow block:** 1 cognitive block (The block occurred exclusively while *searching* for the appointment record, but reading and separating the patient/doctor information on the card was seamless once found).

### 2. Attribute: Learnability
### Scenario: Intuitive Navigation (Discovery)
- **Errors:** 0 (Did not enter unintended sections like "Records" or "Dependents" when seeking to schedule an appointment).
- **Questions:** 0 disorientation questions asked.
- **Task Efficiency:** Gained direct entry via the prominent "Book an appointment now" button on the home dashboard.

### Scenario: Clear Form Flow
- **Click Count:** Flow completed within the minimum structural taps required by the 4 sequential dropdown form fields.
- **Drop-off Rate:** 0% (Successfully finalized the scheduling form in its entirety).

### Scenario: Recognition of Primary Action (Action Button)
- **Visibility:** Yes, visually identified the action trigger button to initiate the scheduling process.
- **Questions:** 0 questions about how to begin a new appointment.
- **Errors:** 0 (Did not tap on empty layout sections).

### Scenario: Learning "Progressive Disclosure"
- **Flow block:** 0 blocks or freezes (Waited for the available doctor index to fetch after sequentially entering the target date and prior filters).
- **Comprehension:** Yes, understood the downward form hierarchy needed to populate conditional data rows.
- **Efficiency:** Forward progress without backing out of filters.

### Scenario: Use of Date Selector (Digital Calendar)
- **Errors:** 0 freezes or selection faults working within the active calendar days of the current month (May).
- **Questions:** 0 questions regarding inner navigation rules of the May calendar window.
- **Completion:** Yes, pinned the desired date (May 29) accurately on her first attempt.

### Scenario: Specific Doctor Search
- **Visibility:** Yes, recognized the interactive dropdown picker tool and the adjacent arrow indicator component.
- **Click Count:** 2 clicks (1 to open the doctor picker pool list and 1 to confirm the target doctor choice).
- **Errors:** 0 accidental taps outside target list items.
- **Questions:** 0 questions on how to modify the assigned healthcare professional.
- **Recovery:** Selection and navigation completed seamlessly without dropdown lockups.

### 3. Attribute: Error Protection
### Scenario: Recovery from "No Results"
- **Recovery:** Upon booking the appointment and returning to the main menu dashboard, the layout briefly displayed a blank "No results" state. The user correctly recognized the data-fetch latency and switched between tab items to manually trigger a data sync.
- **Comprehension:** Understood that this represented visual state rendering latency rather than a loss of network connectivity.

### Scenario: Confirmation of Irreversible Action
- **Errors:** 0 accidental cancellations (The cancellation workflows triggered in Task 7 were explicit and intentional).
- **Recovery:** Yes, correctly interacted with the modal confirmation pop-up window prompt box.

### Scenario: Prevention of Past Appointments
- **Errors:** During Task 5, when attempting to choose a past month (April), the built-in calendar rules blocked retrogressive selections. The user recognized this lock and verbally stated: "It's fine that it doesn't let you book if it has already passed."
- **Questions:** 0 questions; she immediately absorbed the passive visual calendar constraints.
- **Recovery:** Safely moved past the action independently, respecting the application's underlying business rules.

### 4. Attribute: Satisfaction
### Scenario: Sense of Achievement
- **Completion:** Completed successfully. This user had no registered family dependents active on her profile record ("Has family members registered as beneficiaries: No"). Thus, she executed the test cancellations directly upon her own primary account flow, concluding the evaluation smoothly.
- **Questions:** 0 queries regarding the final system status.
- **Comprehension:** Correctly identified the updated appointment status and verified the transaction endpoint inside the user interface.

---
## Usability Metrics Table per Task

| Module           | Task                                                       | Completed? (Yes/No) | No. Clicks | No. Questions | No. Errors / Stumbles |
| :--------------- | :--------------------------------------------------------- | :-----------------: | :--------: | :-----------: | :-------------------: |
| **Login**        | **Task 1:** Log in with credentials                        |         Yes         |     5      |       0       |           1           |
| **Login**        | **Task 2:** Restart the application (Validate persistence) |         Yes         |     2      |       0       |           0           |
| **Appointments** | **Task 1:** Book primary medical appointment               |         Yes         |     8      |       2       |           0           |
| **Appointments** | **Task 2:** Verification of appointment success in list    |         Yes         |     3      |       0       |           1           |
| **Appointments** | **Task 3:** Visualization of basic data on card summary    |         Yes         |     0      |       1       |           0           |
| **Appointments** | **Task 4:** Visualization of full appointment details      |         Yes         |     8      |       1       |           1           |
| **Appointments** | **Task 5:** Attempt to book in past month (April)          |         Yes         |     3      |       0       |           1           |
| **Appointments** | **Task 6:** Book appointment for beneficiary dependent     |         Yes         |     4      |       0       |           0           |
| **Appointments** | **Task 7:** Cancellation of both medical appointments      |         Yes          |     6      |       0       |           1           |