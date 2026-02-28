## Data Collection Based on the Nielsen and Ramdhani Methodology

- **Field Observation:** Observing how maintenance workers currently request an appointment (e.g., going in person to a service window). This is relevant because it allows us to see real behaviors and frustrations that are not expressed in an office setting.
- **Contextual Interviews:** Conversations held at the user's workplace to understand why they prefer certain methods over others. This helps build the "body" of the Persona with data from everyday life.
- **Use Scenario Mapping:** Documenting the flow a user follows from the moment they experience a symptom until they receive their medication. This is vital for identifying where user behavior conflicts with technical requirements (such as the lack of an institutional email account).

These elements are critical because our project aims for inclusion. Without understanding the behavior of those who do not use institutional technology, we would design a system that only serves a specific group. The relevance lies in bridging the gap between manual and digital procedures for all segments of the university community.

## Specific Examples of Persona Usage

### CASE 1

**Persona: "Don José, the Maintenance Worker"**
**Profile:** 52 years old, 20 years at UADY. Does not use a computer at work and does not remember his Microsoft password because he rarely uses it.
**Goal:** Schedule an appointment for his daughter (a listed beneficiary) without having to ask for time off during his shift to go to the service window in person.
**Impact on the Product:** The use of this Persona will directly impact the **Login and Authentication module:**

- Design Change: Instead of requiring login exclusively through  
  Microsoft (as seen in the original proposal), the team decides to
  implement an alternative access method using an Employee Number and  
  Identity Validation via SMS or CURP.

This approach ensures that the product is not just a tool for administrative staff, but an improved system for the entire university community.

### CASE 2

**Persona: "Elena, Senior Faculty Member"**
**Profile:** 62 years old, tenured professor with 35 years of experience. Uses a computer for her work but prefers to print her documents. She has tired eyesight and feels anxious when an app has too many notifications or hidden menus.
**Goal:** Manage her own annual medical pass and that of her husband (a listed beneficiary) independently, without having to ask her assistants for help or go in person to the personnel offices.

**Impact on the Product:** The inclusion of "Dr. Elena" **will impact the Visualization and Navigation module:**

- **Flat Information Architecture:** Complex menus and hidden touch
  gestures will be avoided, opting instead for large, fixed buttons
  with clear text labels (e.g., "Schedule Appointment" instead of just
  a calendar icon).
- **Visual Accessibility:** The system will include a default "Easy Reading
  Mode" or dynamic font size adjustment, ensuring that staff in this
  age group can read their prescriptions and reference numbers without
  difficulty.
- **Safety Confirmation:** Clear confirmation messages will be implemented
  after each action (e.g., "Your appointment has been successfully
  saved"), reducing the technological anxiety of not knowing whether
  the process was completed correctly
