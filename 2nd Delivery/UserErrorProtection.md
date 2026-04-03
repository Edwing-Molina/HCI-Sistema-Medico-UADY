
# Error Protection Attribute

## 1. Detailed Description of the Attribute

**Error Protection** is the ability of a system to **anticipate human mistakes**.  
It is divided into three main dimensions:

### Constraining
Limiting the user’s options to only those that are valid at a given moment.

**Example:** disabling the **“Schedule”** button if no date has been selected.

### Warning
Alerting the user when an action appears unusual or potentially risky.

**Example:** a warning message when scheduling an appointment and selecting a **pediatrics specialty for an adult patient**.

### Confirmation
Requesting explicit verification before executing **irreversible or high-impact actions**.

**Example:** a **Cancel** button that triggers a confirmation message.

---

# 2. Evaluation Questions (Checklist)

## a. Ease of Input (Smart Controls)

**Question for the user**

> “When choosing a date or time for an appointment, did you feel that the system made the selection easier, or were you worried about entering something in the wrong format?”

**Objective**

Evaluate whether the use of **pickers or selectors** eliminated the cognitive load of remembering formats (e.g., **DD/MM/YYYY**) and whether the user perceived that assistance.

---

## b. Real-Time Guidance

**Questions for the user**

> “While selecting the appointment data or date, did you notice whether the system guided you or whether you felt restricted in what you could type?”

> “Did that make you feel more confident about the information you were entering?”

**Objective**

Determine whether **dropdown menus** are perceived as a **visual and restrictive aid** that prevents errors before pressing **Submit**.

---

## c. Validation of Sensitive Data (Outlier Values)

**Questions for the user**

> “If, due to distraction, you entered data or a value that does not make sense, would you expect the application to stop you?”

> “What type of notification would make you feel that the system is protecting you rather than simply reprimanding you?”

**Objective**

Explore the user’s **trust in the system’s intelligence** to detect logical errors that could be dangerous in a **healthcare context**.

---

## d. Irreversible Actions (Step Confirmation)

**Questions for the user**

> “When trying to delete a record or cancel an appointment, did you feel that the process was too fast, or that the system ensured you truly wanted to do it?”

> “Was the confirmation request clear to you?”

**Objective**

Validate whether **confirmation dialogs** are perceived as **necessary protection** or as an **unnecessary obstacle**.

---

## e. Autonomy in Problem Resolution (Avoiding Dependency)

**Questions for the user**

> “If the system shows you an error, do you feel it provides clear clues to fix it yourself, or do you feel the need to ask someone else how to proceed?”

> “When the issue occurred, did you quickly see how to return to the previous state, or did you feel ‘stuck’ on a screen without knowing which button to press?”

> “Was it easy to identify exactly which data or action caused the problem, or did you have to review the entire screen to guess what was wrong?”

> “Did the message displayed on screen make you feel that the system was guiding you toward a solution, or did you feel that it simply stopped you without explaining how to move forward?”

**Objective**

Evaluate whether **error messages are informative enough** and whether the **visual feedback** helps the user recover without depending on **technical support** or external assistance.

---

# 3. Metrics

These metrics provide an **objective view of how safe the design is**, especially in critical environments such as a **medical application**.

# A. Error Rate per Task (ERT)

## Description

A **frequency metric** indicating how many obstacles an average user encounters when trying to achieve a goal.  
It helps identify which parts of the workflow are **confusing or prone to failure**.

## How to Measure It

Through **moderated or recorded usability testing**, counting incorrect actions such as:

- Clicking non-clickable areas  
- Entering invalid data  
- Failed navigation

## Formula

$$
ERT = \frac{E_{total}}{T_{completed}}
$$

## Required Numerical Values

- $E_{total}$: Total errors committed by all participants  
- $T_{completed}$: Total number of tasks successfully completed

## Example Application

If testing the **Patient Registration** workflow with **5 users** results in:

- **15 errors**
- **5 completed tasks**

Then:

$$
ERT = \frac{15}{5} = 3.0
$$

An **ideal value** is usually **< 0.5**.

# B. Error Severity Index (ESI)

## Description

Weights detected errors according to their **impact**.  
Not all errors are equal: a **spelling mistake** is minor, but choosing the **wrong medical specialty** could be critical.

## How to Measure It

Classifying each detected error during testing on a **scale from 1 to 4**.

## Formula

$$
ESI = \sum (n_i \times w_i)
$$

## Required Numerical Values

- $n_i$: Number of errors found at level $i$  
- $w_i$: Weight assigned to that level

Example severity weights:

| Level | Weight |
|------|------|
| Minor | 1 |
| Moderate | 2 |
| Critical | 3 |
| Catastrophic | 4 |

## Example Application

If testing detects:

- **10 minor errors**
- **1 critical error**

$$
(10 \times 1) + (1 \times 3) = 13
$$

This index helps determine whether the **product can be released** or if the **risk is too high**.

# C. Alert Interruption Rate (AIR)

## Description

Measures **cognitive load**.  
Evaluates whether the system protects users through **intelligent design** or **overloads them with alerts**.

## How to Measure It

Count how many times a **dialog box or alert** interrupts the workflow.

## Formula

$$
AIR = \frac{A_{int}}{P_{total}}
$$

## Required Numerical Values

- $A_{int}$: Number of alerts or confirmation dialogs  
- $P_{total}$: Number of steps required to complete the workflow

## Example Application

If scheduling an appointment requires **6 steps** and the system shows **3 alerts**:

$$
AIR = \frac{3}{6} = 0.5
$$

A high value indicates **alert fatigue**, meaning users stop reading warnings.

# D. Successful Recovery Rate (SRR)

## Description

Evaluates the **system’s resilience**.  
If prevention fails, it measures how easily users can **correct errors without frustration**.

## How to Measure It

Observe how many errors users correct themselves after receiving **error messages** or using **Undo**.

## Formula

$$
SRR = \left( \frac{E_{corr}}{E_{total}} \right) \times 100
$$

## Required Numerical Values

- $E_{corr}$: Number of errors corrected by the user  
- $E_{total}$: Total number of errors committed

## Example Application

If a user commits **10 errors** and corrects **8**:

$$
SRR = 80\%
$$

A low value indicates **unclear error messages** or **poor recovery design**.

---

# Summary for the Report (Target Values)

| Metric | Focus | Suggested Target |
|------|------|------|
| **ERT** | Failure frequency | < 0.5 per task |
| **ESI** | Failure impact | Downward trend |
| **AIR** | Workflow / Cognitive load | < 0.2 per step |
| **SRR** | Error correction capability | > 90% |
