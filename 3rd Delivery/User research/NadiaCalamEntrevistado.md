# Software Quality and Usability Evaluation - Nadia Calam

## I. Module: Login

### 1. Attribute: Error Protection

### Scenario: Email Format Validation

- **Errors:** 0 attempts (The user entered her institutional email address with the correct format on the first attempt).
- **Message Comprehension:** Not applicable (The format error message was not triggered).
- **Recovery:** 0 (Did not require fixing the email format).

### Scenario: Credential Error Feedback

- **Errors:** 0 attempts (The user entered her correct email and password directly).
- **Message Comprehension:** Not applicable (The credential error message was not triggered).
- **Recovery:** Not applicable.

### Scenario: Empty Field Submission

- **Errors:** 0 attempts (The user did not attempt to press the login button with empty fields).
- **Message Comprehension:** Not applicable.
- **Recovery:** Not applicable.

### 2. Attribute: Accessibility

### Scenario: Interface Scaling for Older Adults

- **Visibility:** The user perfectly visualized the text fields and labels in their default size without needing to force zoom.
- **Layout Integrity:** The elements of the login interface maintained their standard alignment and correct proportions.

### Scenario: Color-Independent Error Messages

- **Message Comprehension:** Not applicable (No validation errors occurred during access).
- **Visibility:** Not applicable.

### Scenario: Keyboard Navigation

- **Task Completion:** The user completed the login by directly pressing the on-screen button after triggering the institutional validation.
- **Errors:** 0 (There were no interruptions or failures with the device's virtual keyboard).
- **Efficiency:** Continuous interaction and optimal execution time within the flow.

### 3. Attribute: Learnability

### Scenario: Login Flow Recognition

- **Task Completion:** Yes, the user identified the login button with Microsoft instantly upon opening the application.
- **Efficiency:** Immediate access without visual recognition pauses.
- **Errors:** 0 (Did not interact with incorrect components on the welcome screen).

### Scenario: Login Loading State Visibility

- **Errors:** 0 (Did not press the button repeatedly during the waiting time).
- **Awareness:** Yes, the user recognized the loading state and waited calmly for the server response.

### Scenario: Password Correction

- **Errors:** 0 corrections (Entered the exact character sequence of her password on the first attempt).
- **Completion:** Yes, completed the authentication successfully.
- **User Reaction:** Fluid and without hesitation during data capture.

### 4. Attribute: Satisfaction

### Scenario: Session Persistence

- **Task Completion:** Yes, after performing a forced background close (Task 2), the system kept the token active and loaded the Dashboard immediately upon reopening the app.
- **User Reaction:** The user proceeded directly to the next module without showing surprise regarding the persistence.

### Scenario: Interface Trust and Professional Appearance

- **Perceived Trust:** High (The use of the integrated institutional login view transmits security to the user).
- **Message Comprehension:** Yes, she clearly understood that this was the gateway to the university medical system.

---

## II. Module: Appointments

### 1. Attribute: Accessibility

### Scenario: Motor Precision and Fatigue

- **Errors:** 0 clicks outside the targets or on adjacent controls.
- **Task Completion:** Yes, selected all parameters from the dropdown menus with precision and ease.
- **Visibility:** No coordination difficulties or visual fatigue were observed when pressing the form buttons.

### Scenario: Visual Readability (Presbyopia)

- **Message Comprehension:** The user identified and read without problems the technical error message exposed in Task 7 after the backend crash during cancellation.
- **Visibility:** Did not require bringing the device close to her face at any moment to interpret the readable texts of the appointments.

### Scenario: Outdoor Contrast and Visibility

- **Visibility:** Not applicable (The evaluation was conducted in an indoor space with stable lighting conditions).
- **Message Comprehension:** Validated the status "Requested" on her card when updating the interface.
- **Questions asked:** None regarding contrast visibility.

### Scenario: Backwards Navigation (Cognitive)

- **Awareness:** Yes, the user skillfully moved between the different tabs of the bottom menu and back buttons to force the update of the list.
- **Abandonment Rate:** 0% (Remained active within the test flow).
- **Questions asked:** None.

### Scenario: Logical Reading Order (Assisted/Cognitive)

- **Message Comprehension:** Yes, she correctly interpreted the structured appointment data on the screen.
- **Questions asked:** No doubts about the schedule, doctor, or specialty consulted.
- **Flow block:** 0 (Correctly separated the patient information from the doctor's name).

### 2. Attribute: Learnability

### Scenario: Intuitive Navigation (Discovery)

- **Errors:** 0 (Located the golden button "Book an appointment now" directly from the main screen without getting lost in other sections).
- **Questions:** 0 disorientation questions in the interface.
- **Task Efficiency:** Immediate and direct access to the booking flow.

### Scenario: Clear Form Flow

- **Click Count:** Completed the selection of the integrated selectors using the exact steps established by the app design.
- **Drop-off Rate:** 0% (Finalized the complete data capture process for the appointments).

### Scenario: Recognition of Primary Action (Action Button)

- **Visibility:** Yes, the visual design of the main button allowed the user to quickly identify it as the required action.
- **Questions:** 0 questions on how to initiate the creation of a new appointment.
- **Errors:** 0 (Did not press dead or inactive areas of the list).

### Scenario: Learning "Progressive Disclosure"

- **Flow block:** 0 blocks (Assimilated that loading available doctors depended on the previous sequential selection of the date and earlier filters).
- **Comprehension:** Yes, completed the form in a top-down manner without skipping steps.
- **Efficiency:** Continuous progress through conditional fields.

### Scenario: Use of Date Selector (Digital Calendar)

- **Errors:** 0 blocks operating the component within the working day range of the current month.
- **Questions:** 0 questions about the internal functioning of the calendar for the month of May.
- **Completion:** Yes, selected the requested days (May 29 and 27) directly.

### Scenario: Specific Doctor Search

- **Visibility:** Yes, recognized the interactive control to open the list of doctors and change the default option.
- **Click Count:** 2 clicks (1 to display the doctor selector and 1 to confirm the doctor's name).
- **Errors:** 0 wrong clicks on contiguous lines.
- **Questions:** 0 questions on how to modify the assigned doctor.
- **Recovery:** Fluid and effective selection of Dr. Herrera and Dr. Fuentes.

### 3. Attribute: Error Protection

### Scenario: Recovery from "No Results"

- **Recovery:** Upon returning to the appointments module and seeing the blank screen with the legend "No results", the user interpreted the synchronization delay and switched between app sections to update the list.
- **Comprehension:** Understood that the appointment was in the process of loading in the app view.

### Scenario: Confirmation of Irreversible Action

- **Errors:** 0 accidental deletions (The executed cancellations corresponded to the test instructions).
- **Recovery:** Yes, confirmed the action through the pop-up modal assertively.

### Scenario: Prevention of Past Appointments

- **Errors:** In Task 5, when trying to interact with the month of April (past), the user noticed that the calendar blocked backward navigation.
- **Questions:** 0 questions, interpreted the restrictive behavior of the calendar component instantly.
- **Recovery:** Desisted immediately from the action and autonomously identified the business rule restriction.

### 4. Attribute: Satisfaction

### Scenario: Sense of Achievement

- **Completion:** Partially completed. Successfully completed the bookings and the first cancellation (primary holder), but the overall flow was interrupted by the system collapse during the beneficiary's cancellation.
- **Questions:** Did not ask questions, but viewed the SQL exception dialog box.
- **Comprehension:** Correctly registered the first appointment in the history, but finished the test viewing the critical error dialog box (Something went wrong).

---

## Usability Metrics Table per Task

| Module           | Task                                                       | Completed? (Yes/No) | No. Clicks | No. Questions | No. Errors / Stumbles |
| :--------------- | :--------------------------------------------------------- | :-----------------: | :--------: | :-----------: | :-------------------: |
| **Login**        | **Task 1:** Log in with credentials                        |         Yes         |     3      |       0       |           0           |
| **Login**        | **Task 2:** Restart the application (Validate persistence) |         Yes         |     2      |       0       |           0           |
| **Appointments** | **Task 1:** Book primary medical appointment               |         Yes         |     7      |       0       |           0           |
| **Appointments** | **Task 2:** Verification of appointment success in list    |         Yes         |     1      |       0       |           0           |
| **Appointments** | **Task 3:** Visualization of basic data on card            |         Yes         |     0      |       0       |           0           |
| **Appointments** | **Task 4:** Visualization of full appointment details      |         Yes         |     1      |       0       |           0           |
| **Appointments** | **Task 5:** Attempt to book in past month (April)          |         Yes         |     3      |       0       |           1           |
| **Appointments** | **Task 6:** Book appointment for beneficiary               |         Yes         |     8      |       0       |           0           |
| **Appointments** | **Task 7:** Cancellation of both medical appointments      |         No          |     3      |       0       |           1           |
