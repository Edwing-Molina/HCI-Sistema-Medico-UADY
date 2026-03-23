# Usability Metric Questions — UADY Medical Service App


## 1. Learnability

**Metric:** Average execution time for the first task  
**Goal:** < 3 minutes

---

### 1.1 Test Task

| Field                  | Detail                                                                                                    |
|------------------------|-----------------------------------------------------------------------------------------------------------|
| **ID**                 | T-LEARN-01                                                                                                |
| **Task**               | "Without having used the application before, log in and schedule a General Medicine appointment for tomorrow morning shift" |
| **Target Persona**     | Don José (primary) + Dra. Elena (secondary)                                                               |
| **Requirements Evaluated** | FR02/FR02b (Login), FR07 (Scheduling), FR08 (Campus filtering)                                        |
| **Data to Record**     | Start time, end time, whether completed without assistance                                                |

### 1.2 Post-Task Questions (apply immediately after)

| ID   | Question                                                                                       | Scale                                              | Justification                                                        |
|------|------------------------------------------------------------------------------------------------|----------------------------------------------------|----------------------------------------------------------------------|
| L-01 | "Were you able to complete the task without anyone explaining how to do it?"                   | Yes / No / I needed some help                      | Measures autonomy on first use, core of learnability                 |
| L-02 | "How easy or difficult was it for you to schedule your appointment the first time?"            | 1 (Very difficult) → 7 (Very easy) — SEQ Scale     | Subjective perception of difficulty on first attempt                  |
| L-03 | "Was there any step where you did not know what to do or which button to press?"               | Yes → Which step? / No                             | Identifies exact points of confusion in the flow                     |
| L-04 | "If you had to schedule another appointment tomorrow, would you feel confident doing it alone?" | 1 (Not confident at all) → 5 (Very confident)     | Measures confidence acquired after first use                         |
| L-05 | "What was the first thing you tried to do when you opened the application?"                    | Open-ended question                                | Reveals whether the visual hierarchy correctly guides the user       |

### 1.3 Observation Checklist (for the facilitator)

| Aspect                                                              | Yes | No | Notes |
|---------------------------------------------------------------------|-----|----|-------|
| Did the user identify the login button in less than 10 seconds?     |     |    |       |
| Did the user navigate to the scheduling flow without excessive exploration? |     |    |       |
| Did the user complete the task without asking for help?             |     |    |       |
| Did the user pause for more than 15 seconds on any step? Which one? |     |    |       |
| Did the user attempt to press an incorrect element?                 |     |    |       |
| **Total task time:** _____ min _____ sec                            |     |    |       |

### 1.4 Success Criteria

| Indicator                         | Minimum Threshold | How It Is Calculated                                        |
|-----------------------------------|-------------------|-------------------------------------------------------------|
| Average time for first task       | ≤ 3 minutes       | Average time across all participants                        |
| Completion rate without assistance | ≥ 75%            | Participants who answered "Yes" in L-01 / Total             |
| Average SEQ score (L-02)         | ≥ 5/7             | Average of responses on the 7-point scale                   |
| Confidence for second use (L-04) | ≥ 4/5             | Average of responses                                        |

---

## 2. Error Handling

**Metric:** Error recovery success rate  
**Goal:** > 90%

---

### 2.1 Test Tasks (Provoked Error Scenarios)

| ID       | Error Scenario                        | How It Is Provoked                                          | Requirements Evaluated   |
|----------|---------------------------------------|-------------------------------------------------------------|--------------------------|
| T-ERR-01 | Connection error                      | Disable WiFi/mobile data on the device before scheduling    | FR13, NFR-U-06           |
| T-ERR-02 | Failed login                          | Intentionally enter incorrect credentials                   | FR02/FR02b, NFR-U-06     |
| T-ERR-03 | Cancellation limit reached            | Simulate a user with 3 previous cancellations               | FR11, FR12, NFR-U-06     |

**Instruction for the facilitator:**
> *"Provoke the error in a controlled manner. Observe whether the user reads the message, understands what happened, and manages to continue without assistance."*

### 2.2 Post-Error Questions (apply after each scenario)

| ID   | Question                                                                                          | Scale                                                          | Justification                                                         |
|------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------|-----------------------------------------------------------------------|
| E-01 | "When the error message appeared, did you understand what had happened?"                          | Yes / More or less / No                                        | Measures message clarity (NFR-U-06)                                   |
| E-02 | "Did the message tell you what to do to resolve the problem?"                                     | Yes / No                                                       | Validates that messages include "next step" as required by NFR-U-06   |
| E-03 | "Were you able to resolve the problem and continue using the application?"                        | Yes, on my own / Yes, with help / I could not                  | Directly measures recovery rate                                       |
| E-04 | "How did you feel when the error appeared?"                                                       | 1 (Very frustrated) → 5 (Calm, I knew what to do)             | Measures technological anxiety — critical for Don José                |
| E-05 | "Was the message written in a way you could understand, or did it use technical words?"           | Understandable / Some words I did not understand / I did not understand it | Validates human language (NFR-U-06)                                   |
| E-06 | "In your own words, what did the error message tell you?"                                         | Open-ended question                                            | Verifies real comprehension, not just declarative                     |

### 2.3 Observation Checklist

| Aspect                                                              | Yes | No | Notes |
|---------------------------------------------------------------------|-----|----|-------|
| Did the user read the complete error message?                       |     |    |       |
| Did the user show expressions of confusion or frustration?          |     |    |       |
| Did the user attempt the action suggested by the message?           |     |    |       |
| Did the user recover without facilitator intervention?              |     |    |       |
| Did the user attempt to close the app as a response to the error?   |     |    |       |
| **Recovery time:** _____ sec                                        |     |    |       |

### 2.4 Success Criteria

| Indicator                            | Minimum Threshold | How It Is Calculated                                      |
|--------------------------------------|-------------------|------------------------------------------------------------|
| Unassisted recovery rate             | ≥ 90%            | Participants who answered "Yes, on my own" in E-03 / Total |
| Message comprehension                | ≥ 85%            | Participants who answered "Yes" in E-01 / Total            |
| Next step indication                 | 100%             | All messages must include action — E-02 must be "Yes" for all |
| Average frustration level            | ≥ 3.5/5          | Average of E-04 (above 3.5 = acceptable)                  |

---

## 3. Accessibility (Visual & Technological)

**Metric:** WCAG 2.1 audit compliance score  
**Goal:** AA Level

---

### 3.1 Test Tasks

| ID       | Task                                                                                        | Target Persona | Requirements Evaluated |
|----------|---------------------------------------------------------------------------------------------|----------------|------------------------|
| T-ACC-01 | "Read aloud the information about your next appointment from the screen"                    | Dra. Elena     | NFR-U-01, NFR-U-02     |
| T-ACC-02 | "Increase the text size from your phone settings and verify the app adapts"                 | Dra. Elena     | NFR-U-01               |
| T-ACC-03 | "Log in using your employee number (without institutional email)"                           | Don José       | FR02b                  |
| T-ACC-04 | "From the main screen, find and press the 'Appointments' button"                            | Don José       | NFR-U-03, NFR-U-05     |

### 3.2 Post-Task Questions

| ID   | Question                                                                                              | Scale                                                           | NFR Validated                       |
|------|-------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------|-------------------------------------|
| A-01 | "Were you able to read the information on screen without straining your eyes or bringing the phone closer?" | 1 (Could not read) → 5 (Read perfectly)                        | NFR-U-01 (Legibility)               |
| A-02 | "Did the application colors allow you to clearly distinguish buttons and text?"                        | 1 (Confusing) → 5 (Very clear)                                 | NFR-U-02 (Contrast)                 |
| A-03 | "Were the buttons large enough to press without making mistakes?"                                     | 1 (Too small) → 5 (Perfect size)                               | NFR-U-03 (Interactivity 44x44dp)    |
| A-04 | "When you increased the font size on your phone, did the application adapt correctly?"                | Yes / Partially / No / I do not know how to change the size     | NFR-U-01 (Font scaling)             |
| A-05 | "Were you able to identify yourself in the application without using the Microsoft email?"             | Yes / No / I did not know there was another option              | FR02b (Alternative auth)            |
| A-06 | "Did you always know which section of the application you were in thanks to the bottom menu?"         | Yes, always / Sometimes / No, I got lost                        | NFR-U-05 (Clear navigation)         |
| A-07 | "Did the bottom menu icons have text that helped you know what each button does?"                     | Yes / No / I did not notice                                     | NFR-U-05 (Mandatory text labels)    |

### 3.3 Technical Audit (no user — performed by the team)

| WCAG 2.1 Criterion            | Tool                                          | Threshold                                              | Status            |
|-------------------------------|-----------------------------------------------|--------------------------------------------------------|-------------------|
| Color contrast (1.4.3)        | Colour Contrast Analyser / Figma plugin       | ≥ 4.5:1 normal text, ≥ 3:1 large text                 | ☐ Pass / ☐ Fail   |
| Text scaling (1.4.4)          | Manual test: scale to 200% on device          | No loss of content or functionality                    | ☐ Pass / ☐ Fail   |
| Minimum touch area (2.5.8)    | Figma inspection / prototype measurement      | ≥ 44x44 dp on all interactive elements                 | ☐ Pass / ☐ Fail   |
| Text labels on icons (1.1.1)  | Visual review                                 | All nav icons have text                                | ☐ Pass / ☐ Fail   |
| Alternative access method     | Functional verification                       | Login via employee number + SMS/CURP works             | ☐ Pass / ☐ Fail   |
| Non-technical error language (3.3.3) | Review of all error messages              | No technical jargon, includes next step                | ☐ Pass / ☐ Fail   |

### 3.4 Success Criteria

| Indicator                            | Minimum Threshold | How It Is Calculated                                    |
|--------------------------------------|-------------------|---------------------------------------------------------|
| Perceived legibility (A-01)          | ≥ 4/5            | Average of responses                                    |
| Perceived contrast (A-02)            | ≥ 4/5            | Average of responses                                    |
| Perceived touch area (A-03)          | ≥ 4/5            | Average of responses                                    |
| Functional font scaling (A-04)       | 100% "Yes"       | All must confirm adaptation                             |
| Successful alternative auth (A-05)   | ≥ 90% "Yes"      | Participants with Don José profile                      |
| WCAG audit                           | 100% Pass        | All technical criteria must pass                        |

---

## 4. System Status Visibility (Feedback)

**Metric:** Interface visual response time  
**Goal:** < 5 seconds

---

### 4.1 Test Tasks

| ID        | Task                                                  | What to Observe                                   | Requirements Evaluated |
|-----------|-------------------------------------------------------|---------------------------------------------------|------------------------|
| T-FEED-01 | "Press 'Schedule Appointment' and wait for confirmation" | Does a loading indicator appear? How long does it take? | NFR-U-07, FR07         |
| T-FEED-02 | "Cancel an existing appointment"                      | Does a confirmation modal appear? Is it understandable? | FR10, FR05, NFR-U-07   |
| T-FEED-03 | "Log out of the application"                          | Does an "Are you sure?" modal appear?              | FR05, NFR-U-07         |

### 4.2 Post-Task Questions

| ID   | Question                                                                                                     | Scale                                                                    | NFR Validated                        |
|------|--------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|--------------------------------------|
| F-01 | "After pressing a button, did you know the application was working or did you think nothing was happening?"   | Yes, I always knew / Sometimes I did not know / I thought it had frozen  | NFR-U-07 (Visual feedback)           |
| F-02 | "Did any animation or loading indicator appear while the app processed your request?"                        | Yes / No / I did not notice                                              | NFR-U-07 (Loading indicator >200ms)  |
| F-03 | "Did the application show you a clear message confirming that your action was successful?"                    | Yes / No / I am not sure if it was completed                             | NFR-U-07 + Satisfaction              |
| F-04 | "When you tried to cancel an appointment, did the app ask you to confirm before doing it?"                   | Yes / No                                                                 | FR10 (Warning modal)                 |
| F-05 | "Did the cancellation confirmation message explain that it counts toward your annual limit?"                 | Yes / No / I did not notice                                              | FR10 (Cancellation warning)          |
| F-06 | "At any point, did you feel anxious because you did not know if the application had done what you asked?"    | 1 (Very anxious) → 5 (Always calm)                                      | NFR-U-07 (Mitigate anxiety)          |

### 4.3 Observation Checklist

| Aspect                                                            | Yes | No | Time (sec) |
|-------------------------------------------------------------------|-----|----|------------|
| Does a loading indicator appear when scheduling?                  |     |    |            |
| Does a loading indicator appear when cancelling?                  |     |    |            |
| Does a confirmation modal appear before cancelling?               |     |    |            |
| Does a confirmation modal appear before logging out?              |     |    |            |
| Does a success message appear post-action?                        |     |    |            |
| Did the user show signs of anxiety due to waiting?                |     |    |            |
| **Time between click and visual feedback:** _____ sec             |     |    |            |

### 4.4 Success Criteria

| Indicator                                | Minimum Threshold | How It Is Calculated                                      |
|------------------------------------------|-------------------|------------------------------------------------------------|
| Average time to visual feedback          | ≤ 5 seconds       | Stopwatch: click → visible indicator                       |
| Loading indicator present (F-02)         | 100% "Yes"        | All actions >200ms must display it                         |
| Success confirmation present (F-03)      | 100% "Yes"        | All flows must confirm                                     |
| Cancellation modal present (F-04)        | 100% "Yes"        | Mandatory requirement FR10                                 |
| Anxiety level (F-06)                     | ≥ 4/5             | Average — must be low                                      |

---

## 5. Cognitive Load Reduction

**Metric:** Perceived mental workload + SUS  
**Goal:** SUS > 80 points

---

### 5.1 Test Tasks

| ID       | Task                                                                                           | What to Observe                                                              | Requirements Evaluated |
|----------|------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------|------------------------|
| T-COG-01 | "Schedule a complete appointment: select patient, specialty, shift, date, and doctor"          | Does the user get confused by the number of steps? Does each screen have ≤3 fields? | NFR-U-04, FR07         |
| T-COG-02 | "Search for a family member by name in the beneficiary list"                                   | Is the filter intuitive?                                                      | FR15, NFR-U-04         |
| T-COG-03 | "Freely navigate through the app for 2 minutes exploring the sections"                        | Did the user become disoriented? Did the bottom menu help?                   | NFR-U-05, FR14         |

### 5.2 SUS Questionnaire (Post-Complete Session)

Apply **at the end of the ENTIRE session**, not after an individual task.

| #      | Question                                                                          | 1 (Strongly disagree) → 5 (Strongly agree) |
|--------|-----------------------------------------------------------------------------------|---------------------------------------------|
| SUS-01 | "I think that I would like to use this application frequently"                    | ① ② ③ ④ ⑤                                  |
| SUS-02 | "I found the application unnecessarily complex"                                   | ① ② ③ ④ ⑤                                  |
| SUS-03 | "I thought the application was easy to use"                                       | ① ② ③ ④ ⑤                                  |
| SUS-04 | "I think that I would need the support of someone to be able to use this application" | ① ② ③ ④ ⑤                                  |
| SUS-05 | "I found the various functions in this application were well integrated"          | ① ② ③ ④ ⑤                                  |
| SUS-06 | "I thought there was too much inconsistency in this application"                  | ① ② ③ ④ ⑤                                  |
| SUS-07 | "I would imagine that most people would learn to use this application very quickly" | ① ② ③ ④ ⑤                                  |
| SUS-08 | "I found the application very cumbersome to use"                                  | ① ② ③ ④ ⑤                                  |
| SUS-09 | "I felt very confident using the application"                                     | ① ② ③ ④ ⑤                                  |
| SUS-10 | "I needed to learn a lot of things before I could get going with this application" | ① ② ③ ④ ⑤                                  |

> **SUS Calculation:** For odd items: (response - 1). For even items: (5 - response). Sum all × 2.5 = Score 0-100.

### 5.3 Complementary Cognitive Load Questions

| ID   | Question                                                                                        | Scale                                                   | NFR Validated                         |
|------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------|---------------------------------------|
| C-01 | "Did you feel there was too much information on any screen?"                                    | Yes → Which one? / No                                   | NFR-U-04 (max 3 fields/screen)        |
| C-02 | "Did the appointment scheduling process seem like it had too many steps?"                       | 1 (Too many) → 5 (Just the right amount)                | NFR-U-04 (Progressive disclosure)     |
| C-03 | "Did you always know where you were in the appointment scheduling process?"                     | Yes / Sometimes / No                                    | NFR-U-04 + NFR-U-05                   |
| C-04 | "Did you have to remember information from a previous screen to complete any step?"             | Yes / No                                                | NFR-U-04 (No reliance on memory)      |
| C-05 | "Did the bottom menu help you always know how to go back or switch sections?"                   | Yes, a lot / Somewhat / No, I got lost                  | NFR-U-05, FR14                        |
| C-06 | "After using the entire application, how mentally tired do you feel?"                           | 1 (Very tired) → 5 (Not tired at all)                   | General cognitive load                 |

### 5.4 Simplified NASA-TLX (Optional)

| Dimension      | Simplified Question                                               | Scale 1-7                        |
|----------------|-------------------------------------------------------------------|----------------------------------|
| Mental Effort  | "How much mental effort did it take to use the application?"      | 1 (None) → 7 (Extremely high)   |
| Frustration    | "How frustrated did you feel during use?"                         | 1 (Not at all) → 7 (Extremely)  |
| Performance    | "How successful do you feel about what you managed to accomplish?" | 1 (Not successful) → 7 (Very successful) |

### 5.5 Success Criteria

| Indicator                                  | Minimum Threshold | How It Is Calculated                                  |
|--------------------------------------------|-------------------|-------------------------------------------------------|
| **SUS Score**                              | ≥ 80/100          | Standard SUS formula                                  |
| Information overload (C-01)                | ≤ 20% "Yes"       | Less than 20% should feel overloaded                  |
| Steps perceived as adequate (C-02)         | ≥ 4/5             | Average of responses                                  |
| Process orientation (C-03)                 | ≥ 85% "Yes"       | Percentage that always knew where they were            |
| Mental fatigue (C-06)                      | ≥ 4/5             | Average — should feel minimally tired                 |
| NASA-TLX Mental Effort                     | ≤ 3/7             | Average — must be low                                 |

---

