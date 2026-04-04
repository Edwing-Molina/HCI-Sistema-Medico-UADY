Aquí tienes la propuesta de métricas para el atributo de **Accesibilidad**, adaptada estrictamente al formato que solicitaste y enfocada en los requisitos de tu app para el personal de la **UADY**.

---

## 1. Detailed Description of the Attribute

**Accessibility** is the degree to which a product can be used by people with the *widest range of characteristics and capabilities*, including those with age-related visual fatigue, low digital literacy, or physical exhaustion.
It is divided into three main dimensions:

### Visual Perception
Ensuring that information and UI components are presentable to users in ways they can perceive, regardless of their visual acuity.

*Example:* Using a **4.5:1 contrast ratio** for the UADY golden brand color so a maintenance worker can read it under bright sunlight or with visual fatigue.

### Physical Operability
Guaranteeing that interface elements can be operated by anyone, including users with reduced motor precision due to age or manual labor.

*Example:* Designing buttons with a minimum area of **44x44 dp** to avoid "fat finger" errors or misclicks.

### Cognitive Clarity
Reducing the mental effort required to understand the interface and its messages, especially for users who do not dominate the digital ecosystem.

*Example:* Using **progressive disclosure** to show only 3 fields at a time, preventing an older adult from feeling overwhelmed during the appointment process.

---

# 2. Metrics

Estas métricas permiten medir de forma objetiva el nivel de inclusión de la app, separando lo que puede auditarse automáticamente de lo que requiere validación con el personal de la universidad.

# A. Contrast Compliance Ratio (CCR) - [Automatic]

## Description
A *technical accessibility metric* that verifies if the text and interactive elements are visible enough against their background to be read by users with moderate visual impairment (WCAG 2.1 AA).

## How to Measure It
Using automated audit tools (Lighthouse, Axe DevTools, or Figma Contrast plugins) to scan all app screens.

## Formula
$$CCR = \left( \frac{E_{pass}}{E_{total}} \right) \times 100$$

## Questions for Evidence Analysis
* *Color Contrast:* Does the UADY golden text on a white background meet the **4.5:1** ratio?
* *State Visibility:* Do disabled buttons or secondary labels remain legible for a user with visual fatigue?
* *Non-Text Contrast:* Do icons and graphical objects have a contrast of at least **3:1** against adjacent colors?

## Required Numerical Values
* $E_{pass}$: Number of UI elements that meet or exceed the 4.5:1 ratio.
* $E_{total}$: Total number of text and icon elements evaluated.

## Example Application
If the *Login* screen has 10 text elements and 8 meet the AA standard:
$$CCR = \left( \frac{8}{10} \right) \times 100 = 80\%$$
An *ideal value* is **100%** for WCAG AA compliance.

---

# B. Touch Target Adherence (TTA) - [Automatic]

## Description
Evaluates the *physical accessibility* of the interface. It measures if buttons are large enough to be pressed easily by users with large hands (maintenance staff) or reduced motor coordination.

## How to Measure It
Through code inspection or UI audit tools, measuring the pixel/dp dimensions of all clickable areas.

## Formula
$$TTA = \left( \frac{T_{valid}}{T_{total}} \right) \times 100$$

## Questions for Evidence Analysis
* *Minimum Size:* Are all buttons, like "Agendar Cita", at least **44x44 dp**?
* *Spacing:* Is there enough "breathing room" between the time-slot pills to prevent accidental clicks?
* *Interactive Scaling:* Do targets remain large enough when the user increases the system font size?

## Required Numerical Values
* $T_{valid}$: Number of interactive targets measuring $\ge$ 44x44 dp.
* $T_{total}$: Total number of interactive elements on the screen.

## Example Application
In the *Appointment Scheduling* screen with 12 time slots, if only 6 meet the size requirement:
$$TTA = \left( \frac{6}{12} \right) \times 100 = 50\%$$
A low value indicates a high risk of user frustration for the maintenance staff.


# C. Human Message Comprehension (HMC) - [Manual / User-Based]

## Description
Measures *cognitive accessibility*. It evaluates if the error messages and instructions use "human" language instead of technical jargon, allowing users to solve problems alone.

## How to Measure It
During usability tests with employees, asking them to explain what an error message means in their own words.

## Formula
$$HMC = \left( \frac{U_{understand}}{U_{total}} \right) \times 100$$

## Questions for Evidence Analysis
* *Clarity:* Did the user understand why the appointment was blocked without asking for help?
* *Actionability:* Does the message "Has excedido el límite..." tell the user exactly what to do next?
* *Tone:* Is the language perceived as helpful rather than punitive or overly technical?

## Required Numerical Values
* $U_{understand}$: Number of users who correctly interpreted the message and the next step.
* $U_{total}$: Total number of users tested.

## Example Application
If 10 cleaning staff members encounter the Microsoft MFA error and only 4 know how to proceed:
$$HMC = \left( \frac{4}{10} \right) \times 100 = 40\%$$
A value **> 90%** is required to ensure the app is "ecosystem independent."

---

# Summary for the Report (Target Values)

| Metric | Dimension | Focus | Suggested Target |
| :--- | :--- | :--- | :--- |
| **CCR** | Visual | WCAG AA Contrast | **100%** |
| **TTA** | Physical | 44x44 dp targets | **100%** |
| **HMC** | Cognitive | Human language | **> 90%** |