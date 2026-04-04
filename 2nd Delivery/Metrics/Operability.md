# Operability Attribute

## 1. Detailed Description of the Attribute

*Operability* is the ability of a system to be *easily operated and controlled* by its users, allowing them to complete their goals with minimum effort, time, and external assistance.
It is divided into three main dimensions:

### Controllability
The user can initiate, navigate, and complete actions without getting stuck or lost.

*Example:* A user selects a specialty, picks a date, chooses a time slot, and confirms — completing the full appointment flow *without encountering dead ends*.

### Efficiency
The system allows users to achieve their goals with *minimum steps and time*.

*Example:* Scheduling an appointment requires only *4 taps* instead of navigating through 10 different screens.

### Self-evidence
The interface communicates its operation clearly enough that users can *work independently without external help*.

*Example:* A first-time user (janitor, 55 years old) can schedule a medical appointment *without asking a coworker* for guidance.

---

# 2. Metrics

These metrics provide an *objective view of how operable the design is*, especially considering that the UADY Medical Service app must serve users with *very different levels of digital literacy*.

# A. Task Completion Rate (TCR)

## Description

An *effectiveness metric* indicating what percentage of users can successfully finish a given task from start to end.
It reveals whether the interface flow is operable enough to *let users achieve their goals*.

## How to Measure It

Through *moderated or recorded usability testing*, counting how many participants complete the task successfully versus how many abandon or fail.

## Formula


$$
TCR = \frac{T_{success}}{T_{total}} \times 100
$$


## Questions for Evidence Analysis

- *Completion Verification:* Did the user reach the final confirmation screen of the task?
- *Abandonment Point:* At which specific step did users who failed stop or give up?
- *Partial Completion:* Did the user complete some steps correctly but fail at a specific point?
- *Profile Difference:* Was there a measurable difference in completion rates between manual workers (Profile 1) and administrative staff (Profile 2)?
- *Retry Behavior:* Did the user attempt the task more than once before succeeding?

## Required Numerical Values

- $T_{success}$: Number of tasks completed successfully
- $T_{total}$: Total number of tasks attempted across all participants

## Example Application

If *10 users* attempt to schedule a medical appointment and *8 complete it* successfully:


$$
TCR = \frac{8}{10} \times 100 = 80\%
$$


A value below the *85% target* indicates that the workflow has operability barriers that prevent task completion.

# B. Average Task Completion Time (ATCT)

## Description

A *temporal efficiency metric* measuring how long it takes users on average to finish a task.
High times suggest *confusing layouts, unclear labels, or excessive steps* in the workflow.

## How to Measure It

Using a *stopwatch or screen recording timestamps*, measuring from the user's first interaction to the final confirmation for each participant.

## Formula


$$
ATCT = \frac{\sum_{i=1}^{N} t_i}{N}
$$


## Questions for Evidence Analysis

- *Time Distribution:* What was the fastest and slowest completion time? Is there a wide variance?
- *Hesitation Points:* Were there visible pauses (>10 seconds) before any specific step?
- *Profile Comparison:* What is the average time difference between Profile 1 (manual workers) and Profile 2 (academic staff)?
- *Learning Curve:* Did users who repeated the task show measurably shorter times on the second attempt?
- *Bottleneck Identification:* Which individual step consumed the most time within the workflow?

## Required Numerical Values

- $t_i$: Time (in seconds) taken by participant $i$ to complete the task
- $N$: Total number of participants who completed the task

## Example Application

If *5 users* complete the appointment scheduling task with times of *95s, 120s, 210s, 150s, and 175s*:


$$
ATCT = \frac{95 + 120 + 210 + 150 + 175}{5} = \frac{750}{5} = 150s
$$


This result (*150 seconds = 2.5 minutes*) is *within the 180-second target*, but the *210s outlier* suggests one user struggled and may represent Profile 1 behavior that requires further analysis.

# C. Interaction Efficiency Ratio (IER)

## Description

A *navigation precision metric* comparing the actual number of steps a user takes against the minimum required.
It reveals *unnecessary detours, repeated actions, and interface confusion*.

## How to Measure It

Define the *optimal path* (minimum steps) for each task beforehand, then count the *actual steps* taken by each user during testing (taps, swipes, screen transitions).

## Formula


$$
IER = \frac{S_{actual}}{S_{optimal}}
$$


## Interpretation Scale

| IER Value | Interpretation |
|-----------|----------------|
| 1.0 | Perfect — user followed the optimal path |
| 1.1 – 1.5 | Good — minor detours only |
| 1.6 – 2.0 | Moderate — navigation issues present |
| > 2.0 | Poor — significant confusion or rework |

## Questions for Evidence Analysis

- *Detour Frequency:* How many times did the user navigate to a wrong screen and have to return?
- *Repeated Actions:* Did the user tap the same button multiple times or re-enter the same data?
- *Menu Confusion:* Did the user open incorrect menu sections before finding the right one?
- *Back Button Dependency:* How many times did the user rely on the back button to correct navigation?
- *Optimal Path Awareness:* After completing the task, could the user describe the correct sequence of steps?

## Required Numerical Values

- $S_{actual}$: Total number of steps performed by the user
- $S_{optimal}$: Minimum number of steps required to complete the task

## Example Application

If the optimal path to schedule an appointment is *6 steps* and a user takes *9 steps*:


$$
IER = \frac{9}{6} = 1.5
$$


This falls at the *upper limit of "Good"*, suggesting the user took minor detours — possibly tapping the wrong specialty first or checking another screen before returning.

# D. User Autonomy Rate (UAR)

## Description

An *independence metric* measuring what percentage of users can complete tasks *without external help*.
This is especially critical for the UADY Medical Service because Profile 1 users (manual workers) may not have a coworker available to assist them when using the app.

## How to Measure It

During *moderated usability testing*, the facilitator records whether each user completes the task independently or requests verbal help, gestures for guidance, or expresses inability to continue.

## Formula


$$
UAR = \frac{U_{independent}}{U_{total}} \times 100
$$


## Questions for Evidence Analysis

- *Help Requests:* Did the user verbally ask the evaluator for guidance at any point?
- *Gestural Confusion:* Did the user look at the evaluator with uncertainty or gesture for help?
- *External Reference:* Did the user attempt to consult a manual, FAQ, or another person?
- *Abandonment Without Help:* Did any user stop entirely and state they could not continue?
- *Profile Gap:* What is the autonomy difference between Profile 1 (manual workers) and Profile 2 (academic staff)?
- *Authentication Barrier:* Did users requiring alternative login (FR02b) need more assistance than Office 365 users?

## Required Numerical Values

- $U_{independent}$: Number of users who completed the task without any assistance
- $U_{total}$: Total number of users who attempted the task

## Example Application

If *10 users* attempt to schedule an appointment and *7 do it without any help*:


$$
UAR = \frac{7}{10} \times 100 = 70\%
$$


This is *below the 80% target*. Breaking down by profile reveals:

| Profile | Independent | Total | UAR |
|---------|-------------|-------|-----|
| Profile 2 (Academic staff) | 4 | 5 | *80%* ✅ |
| Profile 1 (Manual workers) | 3 | 5 | *60%* ❌ |

This gap confirms that the interface needs *additional scaffolding* (clearer labels, guided steps, visual cues) for users with low digital literacy.

---
