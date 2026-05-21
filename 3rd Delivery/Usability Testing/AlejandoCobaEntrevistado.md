
# Software Quality and Usability Evaluation - Alejandro Waldemar Coba Magaña

## I. Module: Login

### 1. Attribute: Error Protection

### Scenario: Email Format Validation

- **Errors:** 0 attempts (The user did not enter an invalid email format during the test).
- **Message Comprehension:** Not applicable (The format error message was not triggered).
- **Recovery:** 0 (Did not require fixing the email format).

### Scenario: Credential Error Feedback

- **Errors:** 0 attempts (The user entered his institutional credentials correctly on the first attempt).
- **Message Comprehension:** Not applicable (The credential error message was not triggered).
- **Recovery:** Not applicable.

### Scenario: Empty Field Submission

- **Errors:** 0 attempts (The user did not try to submit the form with empty fields).
- **Message Comprehension:** Not applicable.
- **Recovery:** Not applicable.

### 2. Attribute: Accessibility

### Scenario: Interface Scaling for Older Adults

- **Visibility:** The user does not have operating system text scaling active, but states in his profile that he prefers text to be slightly larger than normal. He was able to read the login fields without assistance.
- **Layout Integrity:** Elements remained completely intact; there was no overlapping content on the login screen.

### Scenario: Color-Independent Error Messages

- **Message Comprehension:** Not applicable (No error messages were triggered during login).
- **Visibility:** Not applicable.

### Scenario: Keyboard Navigation

- **Task Completion:** The user successfully logged in by pressing the on-screen button using Microsoft SSO integration.
- **Errors:** 0 (No keyboard interaction errors occurred).
- **Efficiency:** Smooth interaction times aligned with standard SSO single sign-on flows.

### 3. Attribute: Learnability

### Scenario: Login Flow Recognition

- **Task Completion:** Yes, the user located the login button instantly.
- **Efficiency:** Immediate discovery of the primary login action button.
- **Errors:** 0 (Did not click on incorrect elements before the login button, though he asked to confirm if that was the correct button).

### Scenario: Login Loading State Visibility

- **Errors:** 0 (Did not tap the button repeatedly while loading).
- **Awareness:** Yes, the user waited patiently for the validation loading process to complete without signs of frustration.

### Scenario: Password Correction

- **Errors:** 0 corrections (Typed his password accurately on the first attempt).
- **Completion:** Yes, successfully completed the login process.
- **User Reaction:** No confusion observed; data entry was straightforward.

### 4. Attribute: Satisfaction

### Scenario: Session Persistence

- **Task Completion:** Yes, when fully closing the application and reopening it (Task 2), the system maintained the active session token and loaded the user profile directly.
- **User Reaction:** The user showed no confusion and proceeded directly into the workflow, assimilating the persistence seamlessly.

### Scenario: Interface Trust and Professional Appearance

- **Perceived Trust:** High (The user perceived the Microsoft/Office 365 integrated institutional login as the easiest and most trustworthy method).
- **Message Comprehension:** Yes, fully recognized the screen as the official gate to the medical system.

---

## II. Module: Appointments

### 1. Attribute: Accessibility

### Scenario: Motor Precision and Fatigue

- **Errors:** 0 accidental clicks on blank areas or adjacent form dropdown selectors.
- **Task Completion:** Yes, precisely selected the target parameters (Specialty, Shift, Date, Doctor, and Time slots).
- **Visibility:** No motor fatigue or extreme screen-to-face proximity was observed during this specific step.

### Scenario: Visual Readability (Presbyopia)

- **Message Comprehension:** The red cancellation limit banner was not triggered, but the technical database error dialog was displayed during Task 7, which the user read aloud textually from the screen. The evaluation guide recorded "No" regarding bringing the phone closer to read small text in the detailed view.
- **Visibility:** The user identified text characters and strings within the standard appointment views without needing to bring the device closer during detailed reading tasks.

### Scenario: Outdoor Contrast and Visibility

- **Visibility:** Not applicable (The user test was conducted inside a controlled indoor environment).
- **Message Comprehension:** Identified his appointment status ("Requested") successfully after manually refreshing the layout list.
- **Questions asked:** None regarding card contrast or text background.

### Scenario: Backwards Navigation (Cognitive)

- **Awareness:** Yes, the user backed out and successfully switched between bottom tab views and interfaces to refresh the status list independently.
- **Abandonment Rate:** 0% (Did not abandon or close the app due to orientation issues).
- **Questions asked:** None regarding how to return to a previous screen.

### Scenario: Logical Reading Order (Assisted/Cognitive)

- **Message Comprehension:** Yes, the user identified and dictated the full details of the appointment once inside the expanded card view.
- **Questions asked:** None concerning schedules or main data fields.
- **Flow block:** 0 (Did not mix up the patient's name with the medical provider's name).

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
- **Completion:** Yes, pinned the desired date (May 29) accurately on his first attempt.

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

- **Errors:** The user tried to interact with the past month (April) during Task 5, and the application calendar component locked retrogressive navigation. The user noted the restriction and stated, "It won't let me move out of the month."
- **Questions:** Requested/suggested that an explicit warning toast or "invalid month" banner notice should pop up instead of the UI remaining completely static.
- **Recovery:** Yes, absorbed the visual restriction and safely re-entered the normal flow without external intervention.

### 4. Attribute: Satisfaction

### Scenario: Sense of Achievement

- **Completion:** Partially completed. Successfully scheduled both appointments (primary cardholder and dependent family member) and completed the primary cardholder cancellation. He was unable to complete the family dependent cancellation due to a structural system crash.
- **Questions:** Did not ask if the transaction was saved, but read aloud the exact unhandled database exception printed on screen during the final step.
- **Comprehension:** Identified the standard "Requested" badge initially, but concluded the test facing a critical system error view ("Something went wrong").

---

## Usability Metrics Table per Task

| Module           | Task                                                       | Completed? (Yes/No) | No. Clicks | No. Questions | No. Errors / Stumbles |
| :--------------- | :--------------------------------------------------------- | :-----------------: | :--------: | :-----------: | :-------------------: |
| **Login**        | **Task 1:** Log in with credentials                        |         Yes         |     3      |       1       |           0           |
| **Login**        | **Task 2:** Restart the application (Validate persistence) |         Yes         |     2      |       0       |           0           |
| **Appointments** | **Task 1:** Book primary medical appointment               |         Yes         |     7      |       0       |           0           |
| **Appointments** | **Task 2:** Verification of appointment success in list    |         Yes         |     1      |       0       |           0           |
| **Appointments** | **Task 3:** Visualization of basic data on card summary    |         Yes         |     0      |       0       |           0           |
| **Appointments** | **Task 4:** Visualization of full appointment details      |         Yes         |     1      |       0       |           0           |
| **Appointments** | **Task 5:** Attempt to book in past month (April)          |         Yes         |     3      |       0       |           1           |
| **Appointments** | **Task 6:** Book appointment for beneficiary dependent     |         Yes         |     8      |       0       |           0           |
| **Appointments** | **Task 7:** Cancellation of both medical appointments      |         No          |     3      |       0       |           1           |
