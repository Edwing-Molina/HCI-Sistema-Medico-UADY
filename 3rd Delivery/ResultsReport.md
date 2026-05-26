## Project Results and Progress Report

### 1. Summary

This report includes the conclusions of the usability tests applied to the UADY medical service app project, as well as the process through which we moved from having only functional requirements and no non-functional requirements before the project development. During the project, we applied the User-Centered Design (UCD) methodology to evaluate the usability of the application.

### 2. User-Centered Design (UCD) Methodology

In the project, we used the following User-Centered Design (UCD) techniques:

#### **Applied Research Techniques:**

- During the project development, we used the Personas technique to better understand the needs of our users. In our case, these were synthetic personas created with AI, and we aimed to create two groups of users (Manual workers and users aged 45–55).
- Key finding: With this technique, we identified which users would most likely use the app and what characteristics they might have based on the group they belonged to.

#### **Design and Prototyping Techniques:**

- In our case, we did not use any design or prototyping techniques because the application was already developed.

#### **Usability Evaluation Techniques:**

- We used usability testing and applied the SUS questionnaire to evaluate the quality attributes we defined.

### 3. Status and Progress by Stages

#### **Stage 1: Discovery and Requirements**

- In the first stage, we identified non-functional requirements and applied the Personas technique to better understand our users.
- Deliverables: [FR & NFR](/1st%20Delivery/Requeriments.md) and [Personas](/1st%20Delivery/Personas.md)

#### **Stage 2: Identification of Metrics and Quality Attributes (Usability)**

- At this stage, since we did not perform prototyping because the application was already completed, we had to move ahead to the next delivery. Therefore, we identified usability quality attributes and some metrics that helped us analyze what we were going to measure and which metrics were more appropriate. At this point, many adjustments were made regarding which metrics would be used, and based on that, the quality scenarios for the usability tests conducted in the next stage began to be planned.
- Deliverables: [Quality Attributes v1](/2nd%20Delivery/Usability_Attributes.md)  
  - Metrics:
[Accessibility](/2nd%20Delivery/Metrics/AccesibilityMetrics.md)
[Operability](/2nd%20Delivery/Metrics/Operability.md)
[Satisfaction](/2nd%20Delivery/Metrics/SatisfactionMetrics.md)
[UserErrorProtection](/2nd%20Delivery/Metrics/UserErrorProtection.md)

- As a result, we obtained well-defined quality attributes and a clearer idea of the metrics we could use: [Final Quality Attributes](/2nd%20Delivery/UsabilityAtributes2ndVersion.md)

#### **Stage 3: Scenarios, Usability Tests, and Results**

- In this final stage, we clearly defined the scenarios to evaluate, which were the login process and appointment scheduling. Metrics and tasks were assigned based on the attributes and modules being evaluated. Then, a testing protocol was created to guide the usability tests and ensure that everything went smoothly, along with forms to make the usability testing process more dynamic and faster due to limited time. A participant profile form was also created to identify characteristics of the people who participated in the tests. Finally, evidence such as videos and forms were analyzed, and the results report was prepared.
- Deliverables: [Login Scenarios](/2nd%20Delivery/ScenariosLogin.md), [Appointments Scenarios](/2nd%20Delivery/ScenariosCitas.md), [Testing Protocol](/3rd%20Delivery/TestProtocol.md), [Test Results](/3rd%20Delivery/PersonasAnalysis), [Profile Form](https://forms.gle/RqNNvyqtEQ32J2kz8), [Testing Form](https://forms.gle/4PnoGBmzh3xp19SGA), [SUS Form](https://forms.gle/mEv1rBw8nxUermwg6)

## Team Activity Distribution

The work distribution and weighting are described in the following document:

[Scheduling Activities](/3rd%20Delivery/SchedulingActivities.md)

## Usability Test Results

| Field | Value |
|---|---|
| **Institution** | Autonomous University of Yucatán (UADY) |
| **Evaluated System** | Medical Appointment Module - Functional Application |
| **Tested Modules** | Login and Appointment Scheduling |
| **Evaluation Method** | Usability Testing |
| **Total Participants** | 8 users |
| **Target Population** | Maintenance, Cleaning, and Administrative Staff of UADY |

### 1.1 Methodology

Usability tests were conducted following the **Testing Protocol** established in the project documentation. The protocol included:

- **Login Tasks (2 tasks):** Credential validation, error handling, session persistence
- **Appointment Tasks (7 tasks):** Appointment booking, appointment search, modifications, cancellation
- **Post-Evaluation:** System Usability Scale (SUS) with 10 questions plus 4 qualitative questions

**Population Divided into Two Demographic Groups:**

- Group A (Manual Workers/Younger): Ages 35–45, variable digital proficiency
- Group B (Older Adults): Ages 45–55, low digital proficiency, possible family dependence

### 1.2 Global Quantitative Results

#### System Usability Scale (SUS) - Population Comparison

| Metric | Group A (Manual Workers) | Group B (Older Adults) | Difference |
|---|---|---|---|
| **Average SUS Score** | 77.5 / 100 | 70.0 / 100 | -7.5 points |
| **Score Range** | 40.0 - 100.0 | 68.0 - 75.0 | Greater variability in A |
| **Standard Deviation** | ±23.6 | ±3.2 | Much more consistent in B |
| **Usability Category** | Good (Acceptable) | Marginal (Barely acceptable) | |
| **% above threshold (80)** | Not achieved | Not achieved | Both below |

**Interpretation:**

- Both groups are **below the 80-point threshold** (minimum industry standard)
- Group A shows greater **variability** (some users very satisfied, others very frustrated)
- Group B shows greater **consistency** (uniformly moderately satisfied)
- The difference suggests that age range and digital experience significantly impact usability

#### Task Metrics by Module

**LOGIN:**

| Metric | Group A | Group B |
|---|---|---|
| Completion Rate | 100% (4/4) | 100% (4/4) |
| Average Clicks | 7.3 | 6.1 |
| Average Questions | 0.75 | 0.625 |
| Average Errors | 2.5 | 1.625 |
| Assistance Required | 25% (1 user) | 25% (1 user - Grazielita) |

**APPOINTMENTS:**

| Metric | Group A | Group B |
|---|---|---|
| Completion Rate | 98% (27/28 tasks) | 93% (14/15 tasks*) |
| Average Clicks | 3.8 | 4.1 |
| Average Questions | 0.3 | 0.4 |
| Average Errors | 0.4 | 0.6 |
| Navigational Abandonment Rate | 50-80% while searching for details | 50-80% while searching for details |

*Group B: 1 system error (not the user's responsibility) during dependent cancellation.

**Critical Finding:** The Appointments module is **more successful than Login** in both groups, but it presents common friction in post-booking navigation.

## Comparative Analysis

### 2.1 Comparison of General Metrics

#### Comparative Summary Table

| Aspect | Group A (Manual Workers) | Group B (Older Adults) | Difference | Probable Cause |
|---|---|---|---|---|
| **Average SUS** | 77.5 | 70.0 | -7.5 | Age + Digital Competence |
| **Variability (SD)** | ±23.6 | ±3.2 | Group A +620% | Group A has extremes (40-100) |
| **Clicks in Login** | 7.3 | 6.1 | A uses +1.2 clicks | More attempts in A |
| **Errors in Login** | 2.5 | 1.625 | A: +0.875 errors | More frustration in A → more errors |
| **Clicks in Appointments** | 3.8 | 4.1 | B uses +0.3 clicks | Similar; trivial |
| **Errors in Appointments** | 0.4 | 0.6 | B has +0.2 errors | Small difference |
| **Abandonment Rate (Post-Appointment)** | 50-80% | 50-80% | **SAME** | Common IA problem |
| **Global Completion** | 98% | 93% | A: +5% | System error in B |

**Main Conclusion:** Both groups share similar problems (login, post-booking navigation), but **Group B faces additional friction** related to age and digital experience.

### 2.2 Factorial Analysis: Age vs. Digital Competence

#### Impact of Age

**Quantitative Evidence:**

- Login Clicks: Group A (7.3) vs Group B (6.1) → **Age is NOT a predictor of clicks**
- Errors: Group A (2.5) vs Group B (1.625) → **Age does NOT correlate with more errors**
- SUS: Group A (77.5) vs Group B (70.0) → **There is a difference, but modest (-7.5)**

**Qualitative Evidence:**

- Verónica and Alejandro (older adults) performed comparably to digitally competent younger users
- Grazielita (older adult with low competence) performed worse than User 4 from Group A
- **Conclusion:** Age **is not the determining factor** by itself

#### Impact of Digital Competence

**Quantitative Evidence:**

- Group A user with low competence (SUS 40) vs Grazielita (SUS 68) → **Low competence has greater impact**
- Alejandro (older adult, moderate-high competence): 4 errors → compared with User 1 (young): 0 errors
- Grazielita (older adult, very low competence): 22 errors → vs Verónica (older adult, moderate competence): 3 errors

**Qualitative Evidence:**

- Grazielita explicitly expressed fear of clicking and family dependence
- User 4 (Group A, SUS 40) showed similar frustration
- Verónica and Alejandro (both older but competent) navigated without friction

**Definitive Conclusion:**
**Age is a correlation, not the cause.** The real variable is **digital competence and familiarity with mobile interfaces**.

### 2.3 Shared Strengths (Both Groups)

#### 1. **Trust in Institutional Branding**

- **Both groups:** High trust in UADY + Microsoft SSO
- **Impact:** Compensates for friction in other areas
- **Implication:** Investing in branding is an investment in UX

#### 2. **Acceptance of Business Rules**

- **Both groups:** Immediately understand why they cannot schedule appointments in the past
- **Both groups:** Do not repeatedly click disabled buttons
- **Impact:** No confusion about system restrictions
- **Implication:** Business logic is intuitive; no changes required

#### 3. **Patience with Loading States**

- **Both groups:** 0% repeated clicks while loading
- **Both groups:** Wait patiently
- **Impact:** Loading indicators are effective
- **Implication:** Loading states are well designed

### 2.4 Common Problems (Both Groups)

#### 1. **Login = Critical Entry Barrier**

- **Group A:** 25% required assistance (User 4)
- **Group B:** 25% required assistance (Grazielita)
- **Root Problem:** Virtual keyboard + complex passwords
- **Project Impact:** Reduces adoption rate

#### 2. **Post-Booking Friction (50-80% Abandonment)**

- **Group A:** Users get lost searching for appointment details
- **Group B:** Exactly the same pattern
- **Root Problem:** Confusing Information Architecture in the appointments section
- **Project Impact:** Users complete booking but do not validate success

#### 3. **Lack of Clarity in Transaction States**

- **Both groups:** Do not immediately understand the meaning of "Requested" vs "Scheduled"
- **Both groups:** Ask validation questions ("Was it saved?")
- **Root Problem:** Badges/labels are not explicit
- **Project Impact:** Reduces confidence that the appointment was successfully registered

### 2.5 Critical Differences Between Groups

#### Difference 1: Attitude Toward Exploration

- **Group A:** Some users actively explore; others avoid it
- **Group B:** Most request confirmation before exploring
- **Impact:** Group B requires a more guided interface or tutorial

#### Difference 2: Error Tolerance

- **Group A:** User 1 (SUS 100) made 0 errors; User 4 (SUS 40) made many
- **Group B:** More consistent distribution; range 3-22 errors
- **Impact:** Group B needs stronger error protection (larger buttons, more spacing)

#### Difference 3: Motor Precision

- **Group A:** No reports of motor issues
- **Group B:** Grazielita: 5 accidental clicks
- **Probable Cause:** Post-shift fatigue; less familiarity with touch screens
- **Impact:** Need to increase button target size

## Global Conclusions

### 3.1 Main Conclusion

The **UADY Medical Appointment System fulfills its functional objective** (successful booking, appointment visualization, cancellation) in both populations, **but it presents significant operational friction** that especially affects users with low digital competence, regardless of age.

**Evidence:**

- 98% task completion (Group A)
- 93% task completion (Group B)
- SUS 77.5 and 70.0 (both below target)
- 50-80% post-booking abandonment (both groups)
- 25% require assistance during login (both groups)

**Diagnosis:** The application is **functional but not truly accessible** for all target users.

### 3.2 Determining Factor: Digital Competence > Age

**Research Finding:**

The variable that best predicts performance **is not age, but digital competence**:

- Verónica (54 years old, moderate competence) → SUS ~72, 0 cognitive blocks
- Grazielita (similar age, very low competence) → SUS ~68, 2 cognitive blocks
- User 1 (young) → SUS 100, 0 problems
- User 4 (young) → SUS 40, multiple problems

**Conclusion:**

**Design Implication:** The system must be designed to accommodate the full spectrum of digital competence, **not for a specific age range**.

### 3.3 Overall Satisfaction

**Consistent Qualitative Data:**

- All users confirmed they **would use the app frequently**
- Reason: Severe dissatisfaction with the current system (long waits, unanswered phone calls)
- Everyone perceived the UADY + Microsoft branding as **secure and professional**
- However, they acknowledged that **there are small details to improve**
- Marginal SUS scores (70-77) indicate that the "small details" are actually **significant operational friction**

**Conclusion:** The users’ need (improving the current system) **outweighs the existing friction**, but that **does not mean the UX is optimal**. The gap between SUS 77.5 and the threshold of 80 is critical.

## Proposals

### 4.1 Priority Proposals (P0 - Immediate Implementation)

#### P0.1: Eliminate Login Friction Through Biometrics

**Problem:**

- The virtual keyboard causes multiple typos, frustration, and abandonment
- Users must type email + complex password
- Especially problematic for users with low motor precision

**Proposed Solution: Biometric Authentication**

```text
Improved Flow:
┌─────────────────┐
│ LOGIN SCREEN    │
├─────────────────┤
│                 │
│ ┌─────────────┐ │
│ │ Use Finger  │ │  ← Primary visible button
│ │   Print     │ │
│ └─────────────┘ │
│                 │
│ Or Use Email    │  ← Secondary option
│                 │
└─────────────────┘
````

**Benefits:**

- Eliminates 100% of virtual keyboard problems
- Faster (1 tap vs 50+ taps)
- More secure (biometrics > password)
- Accessible for users of all ages

**Implementation:**

- Integrate with device biometric APIs (iOS Face ID, Android Biometric API)
- Use Microsoft Authenticator as an alternative (already mentioned by participants)
- Maintain email/password option as fallback
- Promote biometrics as the preferred method

**Projected Impact:** +8-10 SUS points

#### P0.2: Immediate Post-Booking Redirection

**Problem:**

- The user successfully completes the booking
- But does not know where to find the appointment
- 50-80% abandonment when trying to validate the appointment
- Uncertainty: "Was it saved?" "Where is it?"

**Proposed Solution: Immediate Visible Ticket**

```text
Improved Flow:

BEFORE (Current):
Step 1: Add specialty
Step 2: Select date
Step 3: Select doctor
Step 4: Confirm
[Screen returns to HOME]
"Where is my appointment?" → User gets lost

AFTER (Improved):
Step 1-4: [same]
[NEW] Step 5: SPLASH SCREEN
┌────────────────────────┐
│   ✅ APPOINTMENT BOOKED │
├────────────────────────┤
│                        │
│  Dr. Juan García       │
│  General Medicine      │
│  📅 May 29, 2026       │
│  🕐 10:20 AM           │
│  📍 Main Campus        │
│  🎟️  Ref: #12345      │
│                        │
│ ┌──────────────────┐   │
│ │ View Details ▶   │ ◄─ Large golden button
│ └──────────────────┘   │
│                        │
│     [Back to Home]     │
│                        │
└────────────────────────┘
```

**Benefits:**

- Immediate visual confirmation of success
- Key information visible at a glance
- User can take a screenshot for reference
- Reduces uncertainty ("Was it saved?")
- Smooth transition to "My Appointments"

**Implementation:**

- Create a modal/full-screen confirmation after appointment creation endpoint
- Show key data: doctor, specialty, date, time, campus
- Include reference number
- "View Details" button navigates to appointment in "My Appointments"
- "Share" button for WhatsApp/SMS
- "Back to Home" button to close

**Projected Impact:** +10-12 SUS points (solves 50-80% post-booking abandonment)

#### P0.3: Increase Contrast and Readability of Appointment Cards

**Problem:**

- Users reported difficulty reading appointment details
- 75% of Group A wears glasses; many requested larger font size
- Current cards likely have low contrast or small text
- Especially affects Group B (older adults)

**Proposed Solution: Appointment Card Redesign**

```text
CURRENT CARD (Inferred - Compact):
┌────────────────────────┐
│ Dr. García | Appt #001 │
│ Gen. Med   │ May 29    │
│ 10:20 AM   │ Campus 1  │
│ Status: ⚪ Requested   │
└────────────────────────┘

IMPROVED CARD (Expanded + Contrast):
┌──────────────────────────────────────┐
│                                      │
│  🏥 SCHEDULED APPOINTMENT            │
│                                      │
│  👨‍⚕️  DR. JUAN GARCÍA                │
│     General Medicine                 │
│                                      │
│  📅 Wednesday, May 29, 2026          │
│  🕐 10:20 AM                         │
│  📍 Main Campus                      │
│                                      │
│  ───────────────────────────────     │
│  Status: ✅ CONFIRMED                │
│  Reference: #001234567              │
│                                      │
│ [View Full Details] [Edit]           │
│                                      │
└──────────────────────────────────────┘
```

**Specifications:**

- Font: +2 sizes compared to current (16px → 18-20px minimum)
- Contrast: 4.5:1 for normal text
- Spacing: Increase padding between elements
- Visual Hierarchy: Use emojis to categorize information
- Color-Coding: States with colors + icons (green, yellow, red)
- Simplification: Show only 5-6 key data points; "View Details" for the rest

**Benefits:**

- Improved readability for users with reduced vision
- More intuitive information with emojis
- Lower cognitive load (less information on main screen)
- Especially beneficial for Group B (older adults)

**Implementation:**

- Redesign Card component in the interface
- Update typography system
- Contrast Ratio Checker
- A/B testing with users from both groups

**Projected Impact:** +5-7 SUS points

### 4.2 Secondary Proposals (P1 - Implement Soon)

#### P1.1: Improve Post-Booking Navigation (IA)

**Problem:**

- After booking, users try to find their appointment
- Confusing Information Architecture
- Active tabs are not clearly distinguishable
- 50-80% abandonment while searching for details

**Proposed Solution: Breadcrumb + Better Tab Distinction**

```text
BREADCRUMB (New):
[Home] > [My Appointments] > [Current Appointment] > [Details]

TABS (Improved):
┌──────────────────────────────────────┐
│ [Book New ⭕] [My Appointments 📋]    │ ← More visible active tabs
├──────────────────────────────────────┤
│ Selected tab content                 │
│                                      │
└──────────────────────────────────────┘

Differences:
- Active tab: Colored background, white text
- Inactive tab: Light gray background, dark text
- Animated underline on active tab
- Emojis for quick identification
```

**Implementation:**

- Add Breadcrumb component
- Increase visibility of active tabs (colored background vs gray)
- Add animated underline
- Use emojis as tab label prefixes
- Test with users to confirm intuitive navigation

**Projected Impact:** +3-5 SUS points

#### P1.2: Protection Against Motor Errors (Increase Target Size)

**Problem:**

- Grazielita (Group B) made 5 accidental clicks
- Likely due to post-shift fatigue and button size
- Hit target too small (< 44x44 px)

**Proposed Solution: Increase Button Sizes**

```text
Current Standard (Inferred): 40x40 px
iOS/Android Recommendation: 44x44 px minimum
Accessibility Recommendation: 48x48 px

PROPOSED INCREASE:
- Primary buttons: 56x56 px (from 44-48)
- Spacing between buttons: +8px
- Increase internal padding

Example. Doctor Selector (Dropdown):
┌────────────────────────────────────┐
│ Doctor (Selector):                 │
├────────────────────────────────────┤
│                                    │
│ □ Dr. Juan García        [▼]       │ ← 56px height target
│                                    │
│ □ Dra. María López       [▼]       │ ← Increased spacing
│                                    │
│ □ Dr. Carlos Pérez       [▼]       │
│                                    │
│          [Confirm]                 │ ← 56x56 button
│                                    │
└────────────────────────────────────┘
```

**Benefits:**

- Reduces accidental clicks
- Better for users with reduced motor precision
- Complies with 48px recommended for a correct vision
- Especially beneficial for Group B

**Implementation:**

- Audit design system: current button sizes
- Increase base size from 44px to 56px
- Increase spacing from 4px to 8px
- Test with users after fatigue

**Projected Impact:** +2-3 SUS points

#### P1.3: Add Interactive Tutorial/Onboarding

**Problem:**

- 50% of Group B expressed fear of exploring
- Some requested confirmation even before obvious buttons
- Lack of initial guidance for low-competence users

**Proposed Solution: Optional First-Run Tutorial**

```text
FIRST RUN EXPERIENCE:

Screen 1: Welcome
┌────────────────────────┐
│  🏥 WELCOME            │
│  UADY Appointment      │
│  System                │
│                        │
│  This app makes        │
│  medical appointment   │
│  booking easier        │
│                        │
│ [Continue] [Skip]      │
└────────────────────────┘

Screen 2: How to Book
┌────────────────────────┐
│ 📋 STEP 1: BOOKING     │
│                        │
│ Tap the golden button  │
│ "Book New Appointment" │
│ on the home screen     │
│                        │
│ [Example Button]       │
│                        │
│ [Continue]             │
└────────────────────────┘

Screen 3: View My Appointments
Screen 4: Cancel Appointment

Final Screen: Get Started
````

**Benefits:**

- Reduces fear and initial uncertainty
- Familiarizes users with the main flows
- Especially valuable for Group B
- Can be skipped by experienced users

**Implementation:**

- Create Tutorial component
- Store "tutorial_completed" flag in localStorage
- Show only on first run
- Keep "View Tutorial" option always available in Help section

**Projected Impact:** +4-6 SUS points (especially for Group B)

#### P1.4: Improve Status Messages with Explicit Banner

**Problem:**

- Alejandro suggested that when booking in a past month is not allowed, it is only grayed out without explanation
- Users may not understand why the action is disabled
- Suggested improvement: explicit banner saying "Appointments can only be booked for future dates"

**Proposed Solution: Toast Notification**

```text
When attempting to navigate to a past month:

┌─────────────────────────────────────┐
│ ℹ️  INFORMATION                     │
├─────────────────────────────────────┤
│ Appointments can only be booked     │
│ for future dates. Please select     │
│ a date in the current or a future   │
│ month.                              │
│                                     │
│             [Understood]            │
│                                     │
└─────────────────────────────────────┘
```

**Benefits:**

- Explains why an action is not allowed
- Reduces confusion
- Improves perception of system communication

**Implementation:**

- Detect attempts to select past months
- Show toast/modal with explanatory message
- Maintain visual restriction (grayed out state)

**Projected Impact:** +1-2 SUS points

### 4.3 Tertiary Proposals (P2 - Consider)

#### P2.1: Add Haptic Feedback to Interactions

**Problem:** Especially for Group B users with reduced motor precision, tactile feedback improves confirmation.

**Solution:** Slight vibration when tapping buttons or selecting dropdowns.

**Benefit:** +1 SUS point, improves perceived responsiveness.

#### P2.2: Option to Increase Font Size Globally

**Problem:** 75% reported visual issues; some need more than the default increase.

**Solution:** Settings > Font Size (Normal / Large / Extra Large)

**Benefit:** +2 SUS points, especially for Group B.

#### P2.3: Dark Mode (Optional)

**Problem:** Some users with visual difficulties prefer dark mode.

**Solution:** Add toggle in Settings.

**Benefit:** +1 SUS point.

### Impact vs. Effort Matrix

| Recommendation                | SUS Impact | Effort   | Priority | Type               |
| ----------------------------- | ---------- | -------- | -------- | ------------------ |
| **P0.1: Biometrics**          | +8-10      | Medium   | CRITICAL | Backend + Frontend |
| **P0.2: Immediate Ticket**    | +10-12     | Low      | CRITICAL | Frontend           |
| **P0.3: Improve Readability** | +5-7       | Low      | CRITICAL | Frontend (Design)  |
| **P1.1: Breadcrumb + Tabs**   | +3-5       | Low      | HIGH     | Frontend           |
| **P1.2: Target Size**         | +2-3       | Low      | HIGH     | Design             |
| **P1.3: Tutorial**            | +4-6       | Medium   | HIGH     | Frontend + Content |
| **P1.4: Toast Notifications** | +1-2       | Very Low | MEDIUM   | Frontend           |
| **P2.1: Haptic Feedback**     | +1         | Low      | MEDIUM   | Frontend           |
| **P2.2: Font Size Settings**  | +2         | Low      | MEDIUM   | Frontend + Backend |

### Projected Impact After Implementation

**Pessimistic Scenario (Only P0):**

- Group A: 77.5 → 85.0 (+7.5 points, +9.7%)
- Group B: 70.0 → 78.5 (+8.5 points, +12.1%)

**Realistic Scenario (P0 + P1):**

- Group A: 77.5 → 88.0 (+10.5 points, +13.5%)
- Group B: 70.0 → 82.0 (+12 points, +17.1%)

**Optimistic Scenario (P0 + P1 + P2):**

- Group A: 77.5 → 90.0 (+12.5 points, +16.1%)
- Group B: 70.0 → 84.5 (+14.5 points, +20.7%)

**Conclusion:** With implementation of P0 (3 critical changes), both groups **reach or exceed the SUS threshold of 80** (acceptable).

## Compliance with Usability Attributes

### 5.1 Measurement Approach

The compliance scores in this section are derived directly from the usability test results. Rather than estimating a global percentage per attribute, each attribute is measured through its associated traceability scenarios. Each scenario has observable pass/fail criteria defined before testing, a corresponding artifact, and an observed value recorded during the sessions. The attribute score is then calculated as:

> **Score = (Passed + Partial × 0.5) / Total scenarios × 100**

A scenario is marked **Passed** when all its key metrics meet the defined threshold. It is marked **Partial** when evidence is mixed (some metrics pass, others do not, or the issue is caused by an external factor such as the virtual keyboard). It is marked **Failed** when at least one key metric falls below the threshold and the cause is attributable to the interface.

This approach makes every percentage traceable to named observations from real participants, avoiding arbitrary estimations.

---

### 5.2 Attribute 1: Accessibility

**Target:** ≥ 80% of scenarios passed

#### Traceability Table

| ID | Scenario | Artifact | Pass criterion | Observed result | Status |
|---|---|---|---|---|---|
| ACC-01 | Motor precision — time slot selector | Pill button | 0 adjacent touch errors; ≥90% first-attempt completion | 5 accidental taps (Grazielita); 87.5% first-attempt | **PARTIAL** |
| ACC-02 | Readability — error banner (presbyopia) | Error banner | 100% comprehension without assistance; 0 visual confusion | 100% comprehension; 0 confusions | **PASS** |
| ACC-03 | Outdoor contrast — appointment card | Appointment card | 0 users need to zoom; 100% understand "Requested" status | 75% report visual difficulty; 3/8 asked "Was it saved?" | **FAIL** |
| ACC-07 | Color blindness — login error without color dependency | Login error banner | Error understood via icon+text alone; 100% autonomous correction | 100% understood error; 100% self-corrected | **PASS** |

**How the score was obtained:**

ACC-02 and ACC-07 passed because all 8 participants understood error messages without assistance and corrected their input independently. ACC-01 is marked partial because the completion rate (87.5%) is close to the 90% threshold and the accidental taps were concentrated in a single user (Grazielita), suggesting the issue is severity-bounded rather than systemic. ACC-03 fails because 75% of Group A participants wear corrective lenses and reported visual difficulty with appointment card content, and 3 out of 8 participants asked a validation question about the appointment status, indicating the "Requested" label does not communicate clearly.

**Score: 2 passed + 1 partial × 0.5 = 2.5 / 4 → 62.5%**

**Gap from target: −17.5%** — Significantly below target. The primary causes are insufficient touch target size (ACC-01) and inadequate typographic hierarchy and contrast in appointment cards (ACC-03).

---

### 5.3 Attribute 2: Learnability

**Target:** ≥ 80% of scenarios passed

#### Traceability Table

| ID | Scenario | Artifact | Pass criterion | Observed result | Status |
|---|---|---|---|---|---|
| LRN-01 | Intuitive navigation — appointments module | Bottom menu | 100% locate module without assistance; 0 wrong-module errors | 100% (8/8) located it; 0 navigation errors | **PASS** |
| LRN-03 | Primary button recognition — "Book appointment" | Golden primary button | 0 clicks on empty areas; identified in <5 seconds | 0 misclicks; immediate identification in both groups | **PASS** |
| LRN-05 | Date selector — older adult first use | Calendar component | ≥75% complete without instructions; 0 assistance requests | 87.5% completed unaided; 1 assistance request (Grazielita) | **PASS** |
| LRN-08 | Loading state during login with network latency | Login button — loading state | 0 repeated clicks during load; 100% wait patiently | 0 repeated clicks in both groups; 100% waited | **PASS** |
| LRN-SAT | Post-booking — locate newly booked appointment | Appointments IA | <20% abandonment; 0 validation questions ("Was it saved?") | 50–80% abandonment in both groups; 3/8 asked validation question | **FAIL** |

**How the score was obtained:**

LRN-01, LRN-03, LRN-05, and LRN-08 all passed. The bottom menu labels, the golden primary button color, the calendar navigation, and the loading indicator all performed without measurable friction across both participant groups. LRN-SAT fails because the 50–80% abandonment rate after booking was identical in both groups, meaning this is not a user-competence issue but an architectural deficiency. Users completed the booking task successfully but could not subsequently locate their appointment in the interface, and 3 out of 8 asked explicitly whether their booking had been saved.

**Score: 4 passed + 0 partial = 4 / 5 → 80%**

**Gap from target: 0%** — Meets target exactly. However, the LRN-SAT failure is operationally significant because it affects 50–80% of users after every booking, making it the highest-priority single fix in the system despite the overall attribute score meeting the threshold.

---

### 5.4 Attribute 3: Error Protection

**Target:** ≥ 80% of scenarios passed

#### Traceability Table

| ID | Scenario | Artifact | Pass criterion | Observed result | Status |
|---|---|---|---|---|---|
| ERR-02 | Accidental cancellation — confirmation modal | Confirmation modal | 0 accidental cancellations; 100% read modal | 0/8 accidental cancellations; 100% read modal | **PASS** |
| ERR-03 | Past dates disabled in calendar | Date selector | 0 repeated taps on blocked dates; 100% understand restriction autonomously | 0 repeated taps; 100% understood without explanation | **PASS** |
| ERR-04 | Email format validation | Email input | 0 invalid submissions processed; 100% self-corrected | 0 invalid submissions reached server; 100% self-corrected | **PASS** |
| ERR-05 | Incorrect credentials — clear feedback | Login error message | 100% understand error without assistance; ≤3 consecutive failed attempts average | 87.5% understood unaided; avg. 2.5 errors (Gr. A) / 1.6 errors (Gr. B) | **PARTIAL** |

**How the score was obtained:**

ERR-02, ERR-03, and ERR-04 passed cleanly. No participant accidentally cancelled an appointment, no one repeatedly tapped blocked calendar dates, and all email format errors were self-corrected before submission. ERR-05 is marked partial because, although the error message itself was understood by 87.5% of participants and the average failed attempts (2.5 / 1.6) stayed within bounds, one participant from each group required assistance. Crucially, the root cause is not the error message design but the virtual keyboard causing unintentional typos — the message content is adequate; the input method is the friction point.

**Score: 3 passed + 1 partial × 0.5 = 3.5 / 4 → 87.5%**

**Gap from target: +7.5%** — Above target. Error Protection is the strongest-performing attribute. The system consistently prevents irreversible actions and validates inputs before processing.

---

### 5.5 Attribute 4: Satisfaction

**Target:** SUS average score ≥ 80 points (industry-standard acceptability threshold)

Unlike the other three attributes, Satisfaction is measured directly through the **System Usability Scale (SUS)**, the standardized instrument specifically designed to capture users' subjective perception of a system. The SUS produces a 0–100 score where ≥ 80 is considered "Good" and the accepted industry minimum for a satisfactory product. Using scenario pass/fail criteria for Satisfaction would introduce interpretive bias; the SUS score is the direct, validated measurement for this construct.

#### SUS Results by Group

| Metric | Group A (Manual Workers) | Group B (Older Adults) | Global Average |
|---|---|---|---|
| **Average SUS Score** | 77.5 / 100 | 70.0 / 100 | **73.75 / 100** |
| **Score Range** | 40.0 – 100.0 | 68.0 – 75.0 | — |
| **Standard Deviation** | ±23.6 | ±3.2 | — |
| **Industry Category** | Good (borderline) | Marginal | Marginal |
| **Meets ≥ 80 threshold** | No | No | **No** |

#### How the score was obtained

The SUS was applied individually to all 8 participants immediately after completing the test tasks. Each participant answered 10 standardized Likert-scale questions on a 1–5 scale; scores were then converted to the 0–100 SUS scale using the standard formula. The global average (73.75) is the mean of all individual scores across both groups.

Group A's high variability (SD ±23.6, range 40–100) indicates that satisfaction is strongly tied to individual digital competence rather than to any single interface element. Group B's low variability (SD ±3.2, range 68–75) reflects a consistently moderate experience across all older participants. Both groups fall below the 80-point threshold, confirming that satisfaction is not yet at an acceptable level for the target population as a whole.

Qualitative data from the post-SUS interview supports and contextualizes these scores: all 8 participants stated they would use the app frequently, primarily because the current appointment system (phone-based) generates significantly more frustration. This explains why scores are not lower — users compare the app against a worse baseline, not against an ideal standard. The institutional branding (UADY + Microsoft SSO) also raised perceived confidence, partially compensating for operational friction.

**SUS Score: 73.75 / 100**

**Gap from target: −6.25 points** — Below target. The gap reflects real operational friction (login difficulty, post-booking uncertainty) rather than distrust in the system. Users are willing to use it, but the experience does not yet meet the industry acceptability standard.

#### SUS Score Interpretation Reference

| SUS Range | Adjective Rating | Acceptability |
|---|---|---|
| ≥ 90 | Best Imaginable | Acceptable |
| 80 – 89 | Excellent | Acceptable |
| 70 – 79 | Good | Marginal |
| 60 – 69 | OK | Marginal |
| < 60 | Poor | Not Acceptable |

*Source: Bangor, Kortum & Miller (2009); Sauro & Lewis (2012)*

Both groups fall in the **Marginal** zone. Group A (77.5) is close to the Good/Acceptable boundary; Group B (70.0) sits at the lower end of Marginal. Neither group reaches Acceptable.

---

### 5.6 Global Compliance Summary

The following table consolidates the scores from all four evaluated attributes. Accessibility, Learnability, and Error Protection are measured via scenario pass/fail traceability. Satisfaction is measured directly via the SUS score, normalized to the same 0–100 scale for comparison.

| Attribute | Measurement Method | Score | Target | Gap | Status |
|---|---|---|---|---|---|
| Accessibility | Scenario traceability (2/1/1 of 4) | **62.5%** | 80% | −17.5% | Significantly below |
| Learnability | Scenario traceability (4/0/1 of 5) | **80.0%** | 80% | 0% | At target |
| Error Protection | Scenario traceability (3/1/0 of 4) | **87.5%** | 80% | +7.5% | Above target |
| Satisfaction | SUS score — 8 participants | **73.75%** | 80% | −6.25% | Below target |
| **Global Average** | Mixed (scenarios + SUS) | **75.9%** | **80%** | **−4.1%** | **Below target** |

**Global compliance formula:**

```
(62.5 + 80.0 + 87.5 + 73.75) / 4 = 75.94% ≈ 75.9%
```

**Status: MARGINALLY NON-COMPLIANT** — 4.1% below the 80% minimum target.

---

### 5.7 How to Reach 80% Compliance

The three critical deficiencies identified through the measurement model are:

1. **ACC-03** (appointment card contrast and hierarchy) → P0.3
2. **LRN-SAT** (no post-booking confirmation screen) → P0.2
3. **ACC-01** (insufficient touch target size) → P1.2

For Satisfaction, the SUS gap of −6.25 points is expected to close as the friction points driving low scores are addressed — primarily the login barrier (P0.1) and post-booking uncertainty (P0.2), which were the most frequently cited sources of frustration in post-test interviews. The projected SUS improvement of +8–12 points with P0 implementation would bring the average to approximately 82–86, placing both groups above the 80-point threshold.

Implementing P0 + P1 would improve the affected attributes as follows:

| Attribute | Current | Post P0+P1 (projected) | Change |
|---|---|---|---|
| Accessibility | 62.5% | 75.0% | +12.5% |
| Learnability | 80.0% | 90.0% | +10.0% |
| Error Protection | 87.5% | 90.0% | +2.5% |
| Satisfaction (SUS) | 73.75 pts | ~83–86 pts | +9–12 pts |
| **Global Average** | **75.9%** | **~85.5%** | **~+9.6%** |

**With P0 + P1 implemented, the system would reach approximately 85.5%, surpassing the 80% target.**

---

## General Conclusions

The **UADY Medical Appointment System partially complies with the defined usability attributes**, achieving **74.2% overall compliance** — 5.8% below the 80% target — as measured by direct traceability from scenario observations to attribute scores.

**Attributes above target:**

- Error Protection (87.5%) — highly robust; the system consistently prevents irreversible actions and validates inputs
- Learnability (80.0%) — primary navigation and core interactions are learnable, though post-booking navigation remains a critical failure point

**Attributes below target:**

- Satisfaction (73.75 pts) — high functional completion but low perceived success due to the absence of post-booking confirmation
- Accessibility (62.5%) — barriers persist for users with visual difficulty and reduced motor precision

**The three changes that would most directly close the compliance gap, ordered by projected impact:**

1. Post-booking confirmation screen (P0.2) — resolves SAT-01 and LRN-SAT simultaneously (+16.6% in Satisfaction)
2. Appointment card readability redesign (P0.3) — resolves ACC-03 (+12.5% in Accessibility)
3. Increased button target size (P1.2) — resolves ACC-01 partial status

All three are low-to-medium effort frontend changes. Together, they would bring the global compliance score to approximately 84.6%, making the system genuinely accessible for the full spectrum of digital competence present in the target population.

## References

### A. Participants and Profiles

**Group A (Manual Workers/Younger):**

- 4 users, ages 35-45
- Maintenance, cleaning, and administrative staff
- Digital competence: Variable (40-100 SUS)

**Group B (Older Adults):**

- 4 users, ages 45-55
- Maintenance, cleaning, and administrative staff
- Digital competence: Consistently low-moderate (68-72 SUS)

### B. Measurement Instruments

- System Usability Scale (SUS) - 10 questions
- Task Metrics (clicks, errors, time)
- Qualitative observation (moderator notes)
- Semi-structured post-test interview

### C. Reference Materials

- ManualesAnalisis.md - Detailed Group A analysis
- OlderDemographicGroupAnalysis.md - Detailed Group B analysis
- TestProtocol.md - Complete testing protocol
