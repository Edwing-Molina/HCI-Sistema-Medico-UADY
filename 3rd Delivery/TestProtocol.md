# Testing Protocol: Appointment Module (UADY Medical Service)

## 1. Participant Profile
* **Population:** Maintenance, cleaning, and administrative staff from UADY.
* **Age Range:** 45 to 55 years old.
* **Digital Proficiency:** Low (unfamiliar with the system).
* **Physical Condition:** Potential motor fatigue (post-work shift) and visual fatigue.

## 2. Moderator Instructions
1.  **Neutrality:** Do not assist the user. If they get stuck, ask: *"What do you think should happen here?"*.
2.  **Think Aloud:** Ask the user to narrate what they are seeing and why they are making each decision.
3.  **Environment:** Conduct the test in a location with natural light to validate contrast and visibility.

## 3. Welcome Script (Empathy)
"Hello, thank you very much for helping us. We are testing a new application for UADY medical appointments. We are not evaluating you; we are evaluating the application. If something doesn't go well or you can't find an option, it is not your fault—it means we need to improve the design. Please try to say out loud everything you are thinking or whatever confuses you."

---

## Scripts and Tasks

### Task Script and Execution (Login)

| # | User Task (Script) | Evaluated Scenarios | What to observe (Simple Metrics) |
| :--- | :--- | :--- | :--- |
| **1** | *"Look at the screen. Without touching anything yet, does this look like a secure UADY site to you? Where would you click to enter?"* | Trust / Flow Recognition. | • Does the user identify the institutional logo? (Y/N)<br>• Do they locate the quick Login button?<br>• Do they doubt if it is the official app? |
| **2** | *"Type your email, but intentionally forget to include the '@' or the '.mx'. Then try to log in."* | Email Format Validation. | • Does the error message appear immediately?<br>• Do they understand the error is the email and not the password?<br>• Do they correct it without help? |
| **3** | *"Now clear everything and try to click the 'Login' button with the fields empty."* | Empty Field Submission. | • Does the system block the button or flag an error?<br>• Do they understand which field is missing?<br>• # of extra clicks on the empty button. |
| **4** | *"Enter your email correctly, but type a password that is NOT yours and try to log in."* | Credential Error. | • Is the error message clear? (Y/N)<br>• Do they identify the error icon (without relying solely on the color red)?<br>• # of attempts before asking for help. |
| **5** | <mark>Pending Review</mark> *"Imagine you don't have your glasses. We are going to make the text larger (200%). Can you still read everything clearly, or did the text get crowded?"* | Interface Scaling (Accessibility). | • Do texts or buttons overlap? (Y/N)<br>• Does a scroll bar appear?<br>• Can they read the field labels? |
| **6** | *"Type your real password and, instead of clicking the golden button, use the 'Enter' key on your on-screen keyboard."* | Keyboard Navigation. | • Do they log in upon pressing 'Enter'? (Y/N)<br>• Do they wait for something to happen?<br>• Do they doubt if the keyboard can be used to log in? |
| **7** | *"While the system loads, tell me: Is the app letting you know it's working, or does it look like it froze?"* | Visibility of Loading Status. | • Do they notice the loading indicator (spinner)?<br>• Do they try to click the button multiple times while loading?<br>• Do they recognize that the button was disabled? |
| **8** | *"Close the application completely and open it again. Did it ask for your password again, or did it let you in directly?"* | Session Persistence (Satisfaction). | • Did they go directly to the main screen? (Y/N)<br>• Do they seem relieved not to have to type everything again? |

### Task Script and Execution (Appointments)

| # | User Task (Script) | Evaluated Scenarios | What to observe (Simple Metrics) |
| :--- | :--- | :--- | :--- |
| **1** | *"Imagine you need to schedule a new medical appointment. Where would you press to start?"* | Intuitive Navigation / Primary Action Recognition. | • Did they enter the wrong sections?<br>• # of clicks until opening the form. |
| **2** | *"Fill in the details on the screen to search for a doctor. Use the calendar to choose May 30th."* | Form Flow / Progressive Disclosure / Date Selector. | • Did they skip steps?<br>• Did they try to click grayed-out days on the calendar?<br>• Did they ask how to change the month? |
| **3** | *"In the list of doctors, look for Dr. Augusto Luis and choose the 10:20 AM appointment."* | Specific Doctor Search / Motor Precision and Fatigue. | • Did they notice the doctor menu arrow? (Y/N)<br>• # of "misclicks" on the time slots (pills).<br>• Did they bring the phone closer to their face to read? |
| **4** | *"Now try to search for an appointment for yesterday or for a Sunday. What does the application tell you?"* | Past Appointment Prevention / Recovery from No Results. | • Do they understand why there are no results? (Y/N)<br>• Did they get stuck, or did they try to change the date on their own? |
| **5** | *"You have finished your appointment. Check your appointment list. How do you know your appointment was saved correctly?"* | Sense of Achievement / Logical Reading Order / Outdoor Contrast. | • Do they identify the reference number quickly? (Y/N)<br>• Do they know what "Requested" means?<br>• # of insecurity questions ("Is it done?"). |
| **6** | *"In your appointment list, choose one and find a way to see all the detailed information for that appointment on a full screen."* | Detail Consultation / Learnability / Efficiency. | • # of erroneous clicks outside the card.<br>• Can they tell us the campus name once inside the details? |
| **7** | *"Imagine it’s not for you, but for your child/spouse. Change the patient in the list before searching for the doctor."* | Learnability / Efficiency / Dropdowns. | • Do they identify the "Patient" selector?<br>• # of clicks to open the list.<br>• Do they understand that the data below changes according to the patient? |
| **8** | *"You already searched for doctors, but now I want you to change the default doctor and choose another one from the dropdown list."* | Specific Doctor Search / Dropdowns. | • Do they notice the small menu arrow? (Y/N)<br>• Can they scroll within the list of names?<br>• # of questions: "Where are the other doctors?". |
| **9** | *"Check your appointment list and tell me: What details can you see regarding your appointment?"* | Visual Readability / Reading Order / Context. | • Do they identify the appointment details?<br>• Do they bring the phone closer to read small text? |
| **10** | *"Try to delete the appointment you just made. If a notice appears, read it out loud."* | Confirmation of Irreversible Action / Visual Readability (Presbyopia). | • Do they distinguish the red notice as a warning?<br>• Do they know how to close the notice to NOT cancel? |

---

## 5. Metrics Recording Sheet (For the Evaluator)

Use this table to quickly record the results for each participant:

| Participant | Task # | Task Completed? | # of Clicks | # of Questions/Doubts | # of Errors/Stumbles |
| :--- | :---: | :---: | :---: | :---: | :---: |
| | 1 | [ ] Yes [ ] No | | | |
| | 2 | [ ] Yes [ ] No | | | |
| | 3 | [ ] Yes [ ] No | | | |
| | 4 | [ ] Yes [ ] No | | | |
| | 5 | [ ] Yes [ ] No | | | |
| | 6 | [ ] Yes [ ] No | | | |

---

## 6. Closing and Satisfaction Evaluation (SUS)

Upon completing the tasks, provide the user with a simplified **SUS (System Usability Scale)** format. Since the users have an operational profile, you may read the questions to them and mark their responses on a scale of 1 to 5:

1.  I think that I would like to use this application frequently.
2.  I found the application unnecessarily complex.
3.  I thought the application was easy to use.
4.  I think that I would need the support of a technical person to be able to use this application.
5.  I found the various functions in this application were well integrated.
6.  I thought there was too much inconsistency in this application.
7.  I would imagine that most people would learn to use this application very quickly.
8.  I found the application very cumbersome to use.
9.  I felt very confident using the application.
10. I needed to learn a lot of things before I could get going with this application.

### Qualitative Closing (Post-Test)
After the SUS, ask these 4 open questions. Sometimes they are worth more than any metric:

1. "What do you prefer: for the app to remember you (Persistent Session) or to enter your password every time for security?"
2. "What was the most difficult thing for you to find?"
3. "If you could change anything about the colors or the size of the buttons, what would it be?"
4. "Do you feel confident using this alone at home, or would you ask for help?"

### Acceptance Criteria:
* **Success Metric:** The SUS score must be **higher than 80 points** to consider the appointment module satisfactory for UADY personnel.