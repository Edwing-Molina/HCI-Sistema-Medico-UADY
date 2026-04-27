## Quality Scenarios

### Attribute: Accesibility

### Scenario: Motor Precision and Fatigue
**Context:** A cleaning staff member with tired hands after a work shift attempts to choose a specific time slot.
* **Source:** End user (new).
* **Stimulus:** The user attempts to press the **10:20** time slot "pill" button.
* **Artifact:** Time slot selector.
* **Environment:** User with reduced motor precision.
* **Response:** The touch target area is sufficient for the system to recognize the selection on the first attempt.
* **Metrics:**
    * **Errors:** Number of times they tap the adjacent time slot or the blank space.
    * **Task Completion:** Do they successfully select the intended time?
    * **Visibility:** Do they bring the phone closer to read the time numbers?

### Scenario: Visual Readability (Presbyopia)
**Context:** A 60-year-old maintenance worker attempts to read the instructions of a lockout message.
* **Source:** End user (new).
* **Stimulus:** The red "Cancellation limit" message appears.
* **Artifact:** Error banner.
* **Response:** The contrast and font size allow the instruction to be read without difficulty.
* **Metrics:**
    * **Message Comprehension:** Can the user tell us where to write to get unlocked?
    * **Visibility:** Do they distinguish that the red text is a notice and not a button?

### Scenario: Outdoor Contrast and Visibility
**Context:** A maintenance worker checks if their appointment was accepted while walking through faculty hallways with high natural light (screen glare).
* **Source of Stimulus:** End user (new).
* **Stimulus:** The user attempts to read the appointment status ("Requested") and the reference number.
* **Artifact:** Appointment card in the list.
* **Environment:** High ambient lighting (direct sunlight).
* **Response:** The contrast between the text and the card background allows for data identification without needing to seek shade or turn brightness to maximum.
* **Metrics:**
    * **Visibility:** Does the user have to squint or bring the phone very close?
    * **Message Comprehension:** Can they tell us what the label "Requested" means?
    * **Questions asked:** "Where is my appointment number?"

### Scenario: Backwards Navigation (Cognitive)
**Context:** Don José enters "Schedule appointment" by mistake and wants to go back to see his current appointments, but he is unfamiliar with standard navigation icons.
* **Source of Stimulus:** New user.
* **Stimulus:** The user looks for the button to exit the search screen and return home.
* **Artifact:** Top navigation arrow ("<").
* **Environment:** User disoriented within the flow.
* **Response:** The navigation icon is clear enough and placed in a standard position so the user can return without closing the app.
* **Metrics:**
    * **Awareness:** Do they find the back arrow?
    * **Abandonment Rate:** Do they close the app entirely because they didn't know how to "go back"?
    * **Questions asked:** "How do I get out of here?"

### Scenario: Logical Reading Order (Assisted/Cognitive)
**Context:** The user reads scheduled appointment information to confirm their time.
* **Source of Stimulus:** New user.
* **Stimulus:** The user scans the appointment card visually.
* **Artifact:** Appointment card (Pediatrics).
* **Environment:** Review of important information.
* **Response:** Information is ordered from most to least important (Specialty -> Doctor -> Date/Time), facilitating reading for people unaccustomed to digital forms.
* **Metrics:**
    * **Message Comprehension:** Can they quickly tell the time without reading the whole card?
    * **Questions asked:** "What time did you say it was?" (If they ask, the order isn't clear).
    * **Flow block:** Do they confuse the patient's name with the doctor's name?

---

## 2. Attribute: Learnability

### Scenario: Intuitive Navigation (Discovery)
**Context:** Don José opens the app for the first time and needs to find where to book appointments.
* **Source:** New user.
* **Stimulus:** The user looks for the button to start the scheduling process.
* **Artifact:** Bottom menu.
* **Response:** Thanks to the text labels, the user identifies the "Appointments" module immediately.
* **Metrics:**
    * **Errors:** Do they enter "Files" or "Beneficiaries" before "Appointments"?
    * **Questions:** Do they ask "Where do I click?" or "Where are the appointments?"
    * **Task Efficiency:** Number of clicks from the home screen to opening the scheduling form.

### Scenario: Clear Form Flow
**Context:** The user must fill 4 selectors to see available doctors.
* **Source:** New user.
* **Stimulus:** Completing Patient, Specialty, Shift, and Date.
* **Artifact:** "Schedule appointment" screen.
* **Response:** The flow is logical and doesn't require the user to overthink between steps.
* **Metrics:**
    * **Click Count:** Total taps required to see the list of doctors.
    * **Drop-off Rate:** Do they get frustrated and leave the screen before finishing?

### Scenario: Recognition of Primary Action (Action Button)
**Context:** Don José enters the "Appointments" screen. The screen is either empty or contains old appointments, and he needs to understand how to start the process for a new one.
* **Source:** New user.
* **Stimulus:** The user searches for the trigger to start the scheduling flow.
* **Artifact:** Golden "Schedule appointment" button.
* **Response:** The visual design (golden color and size) allows the user to identify the button as the primary action.
* **Metrics:**
    * **Visibility:** Do they read the button text or tap bottom menu icons trying to find the option?
    * **Questions:** "How do I make a new one?" or "Where do I click?"
    * **Errors:** Do they try to click the "No results" area expecting something to happen?

### Scenario: Learning "Progressive Disclosure"
**Context:** The cleaning worker reaches the form. She expects to see a list of doctors immediately, but the screen is empty until she selects options.
* **Source:** New user.
* **Stimulus:** The user interacts with the Patient and Specialty selectors.
* **Artifact:** Search flow.
* **Response:** The user quickly understands they must fill fields from top to bottom for information (doctors) to appear.
* **Metrics:**
    * **Flow block:** Do they wait for doctors to load without having selected anything?
    * **Comprehension:** Do they read the text "Perform a search to see available doctors" and act accordingly?
    * **Efficiency:** Number of clicks before understanding they must fill the filters.

### Scenario: Use of Date Selector (Digital Calendar)
**Context:** An older adult must choose an appointment day. It is their first time using a touch calendar in an application.
* **Source:** New user.
* **Stimulus:** The user opens the "Appointment Date" selector.
* **Artifact:** Calendar component.
* **Response:** The user understands how to navigate between days and months to select a valid date without external instructions.
* **Metrics:**
    * **Errors:** (N/A)
    * **Questions:** "How do I change to next month?" or "Why won't it let me click Sunday?"
    * **Completion:** Do they set the desired date on the first attempt?

### Scenario: Specific Doctor Search
**Context:** On the results screen, doctor names appear. The user wants to check the availability of a specific doctor from the dropdown list.
* **Source of Stimulus:** New user (no prior experience).
* **Stimulus:** The user interacts with the dropdown menu to change from the default assigned doctor.
* **Artifact:** Doctor dropdown menu (Screenshot 4).
* **Environment:** Normal search operation.
* **Response:** The user identifies the component, opens the list, and successfully selects the desired name.
* **Metrics:**
    * **Visibility:** Does the user identify that the doctor's name has a "little arrow" or that it is an openable menu? (Yes/No). Do they stare at the screen looking for where to change the doctor?
    * **Click Count:** 1 to open the menu + 1 to choose the doctor (Ideal total: 2). How many accidental clicks occur outside the menu?
    * **Errors:** When opening the list, do they select the correct name or accidentally tap the one above/below due to font size? Do they close the menu unintentionally before selecting someone?
    * **Questions:** "Are there more doctors here?", "How do I change the name?", "Why isn't my doctor appearing?" (If they don't know they must click the menu).
    * **Recovery:** If the menu is very long and covers the screen, do they know how to scroll within the list or do they feel stuck?

---

## 3. Attribute: Error Protection

### Scenario: Recovery from "No Results"
**Context:** The user searches for an appointment on a non-business day and the screen remains empty.
* **Source:** New user.
* **Stimulus:** The "No results" magnifying glass appears.
* **Artifact:** Search results screen.
* **Response:** The message is clear enough so the user does not ask what to do next.
* **Metrics:**
    * **Recovery:** Do they try to change the date on their own or stay waiting for something to load?
    * **Comprehension:** Do they understand the problem is the selected day and not the internet connection?

### Scenario: Confirmation of Irreversible Action
**Context:** The user accidentally taps "Cancel appointment" while exploring the list.
* **Source:** New user (exploring).
* **Stimulus:** Pressing the red "Cancel appointment" button.
* **Artifact:** Appointment list.
* **Response:** The system launches a confirmation dialog (Modal) to prevent accidental loss of the appointment.
* **Metrics:**
    * **Errors:** Did they cancel the appointment by mistake?
    * **Recovery:** Do they know how to close the alert to avoid cancellation?

### Scenario: Prevention of Past Appointments
**Context:** Don José wants to book an appointment for a "check-up," but accidentally tries to select yesterday's date on the calendar.
* **Source:** New user.
* **Stimulus:** Interaction with the date selector.
* **Artifact:** Calendar / Date selector.
* **Environment:** User with low digital calendar proficiency.
* **Response:** Past days are disabled (light gray) and do not respond to touch, preventing the scheduling of an invalid appointment.
* **Metrics:**
    * **Errors:** How many times do they try to tap a blocked (gray) day?
    * **Questions:** "Why won't this day select?" or "Is the calendar frozen?"
    * **Recovery:** Do they understand on their own that they must choose a future date or do they stay waiting?

---

## 4. Attribute: Satisfaction

### Scenario: Sense of Achievement (Don José)
**Context:** The user finishes their first booking and wants to be sure they "did it right."
* **Source:** New user.
* **Stimulus:** The system returns the user to the "Appointments" screen after confirmation.
* **Artifact:** Updated appointment list.
* **Response:** The new appointment clearly appears in the list, providing peace of mind.
* **Metrics:**
    * **Completion:** Did they reach the end of the flow?
    * **Questions:** Do they ask "Is it done?" or "Did it save?"
    * **Comprehension:** Do they identify that the "Requested" status means the process was successful?

---

### SUS Format
[SUS](/2nd%Delivery/Metrics/SUS.md)
