
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

# 2. Metrics

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

## Questions for Evidence Analysis

- **Misclick Frequency:** How many times did the user click on non-interactive elements or inactive areas?
- **Format Errors:** How many times did the system reject an input for any reason?
- **Navigation Errors:** How many times did the user deviate from the logical workflow and have to return to the starting point?
- **Error Repetition:** Did the user commit the same error more than once within the same task?

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

## Questions for Evidence Analysis

- **Data Integrity:** Did the error allow information to be saved that could lead to an incorrect appointment? (Level: Catastrophic – 4)
- **Workflow Blockage:** Did the error force the user to restart the application or lose all task progress? (Level: Critical – 3)
- **Operational Obstacle:** Did the error create confusion that required more than three attempts to correct? (Level: Moderate – 2)
- **Cosmetic Error:** Was the error purely visual and did not affect data accuracy? (Level: Minor – 1)

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

## Questions for Evidence Analysis

- **Confirmation Alerts:** How many “Confirm Action” modal windows appeared during the workflow?
- **Validation Interruptions:** How many error dialogs blocked the screen during the process?
- **User Behavior:** Was it observed that the user quickly closed alerts without reading them (click blindness)?

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

## Questions for Evidence Analysis

- **Message Effectiveness:** Did the error message indicate exactly where the failure occurred and how to fix it?
- **First-Attempt Correction:** After seeing the error, did the user correct the data correctly in their next action?
- **Use of Reversal Functions:** Did the user successfully use “Undo” or “Cancel” buttons to revert an error?
- **Help Request:** Did the user verbalize a question or directly ask the evaluator how to proceed?
- **State of Paralysis:** Was there a pause of inactivity longer than 30 seconds after an error message?
- **Use of Manuals:** Did the user attempt to seek help in external documentation or FAQ sections?

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
