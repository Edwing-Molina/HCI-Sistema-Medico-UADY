# Quality Scenarios

---

# 1. Attribute: Error Protection

## Scenario: Email Format Validation

Context:  
An administrative worker attempts to log into the system but accidentally types their institutional email incorrectly.

Source: End user (new).

Stimulus:  
The user enters an email address without the "@" symbol or with invalid characters and presses the "Login" button.

Artifact: Login form email input field.

Environment: Normal operation during login attempt.

Response:  
The system immediately displays a validation message indicating that the email format is incorrect and prevents the login request from being sent.

Metrics:

Errors: Number of attempts where the user tries to submit an invalid email format.

Message Comprehension: Does the user understand that the problem is the email format and not the password?

Recovery: Do users correct the email without asking for help?

---

## Scenario: Credential Error Feedback

Context:  
A user attempts to access their account but mistakenly enters the wrong password.

Source: End user.

Stimulus:  
The user presses the "Login" button after entering incorrect credentials.

Artifact: Login error message.

Environment: Normal login attempt.

Response:  
The system displays a clear message indicating that the email or password is incorrect and allows the user to try again.

Metrics:

Errors: Number of consecutive login attempts before the user corrects their credentials.

Message Comprehension: Do users understand that the issue is incorrect credentials?

Recovery: Do users attempt to retype their password or email after the message appears?

---

## Scenario: Empty Field Submission

Context:  
A distracted user attempts to log in without completing the required fields.

Source: End user.

Stimulus:  
The user presses the "Next" button while input fields are empty.

Artifact: Login form validation system.

Environment: Normal login interaction.

Response:  
The system blocks the login request and highlights the empty fields with clear visual indicators.

Metrics:

Errors: Number of times users attempt to submit the form with empty fields.

Message Comprehension: Do users understand which fields must be filled?

Recovery: Do they complete the missing information without assistance?

---

# 2. Attribute: Accessibility

### *Revisar*

## Scenario: Interface Scaling for Older Adults

Context:  
A 60-year-old maintenance worker increases the font size on their phone to improve readability before logging into the application.

Source: End user with visual limitations.

Stimulus:  
The operating system text size is increased to approximately 200%.

Artifact: Login screen layout.

Environment: Accessibility settings enabled.

Response:  
The interface adapts to the larger text size, allowing the user to scroll without elements overlapping or text being cut off.

Metrics:

Visibility: Can the user read all labels and fields without zooming the screen?

Layout Integrity: Do interface elements remain visible and properly aligned?

---

## Scenario: Color-Independent Error Messages

Context:  
A user with color blindness attempts to identify why their login attempt failed.

Source: End user with visual impairment.

Stimulus:  
An error message appears after an incorrect login attempt.

Artifact: Error message banner.

Environment: User with limited color perception.

Response:  
The system uses icons and descriptive text in addition to red color to indicate the error.

Metrics:

Message Comprehension: Can the user understand the error without relying on color?

Visibility: Do users identify the message as an alert rather than a clickable element?

---

## Scenario: Keyboard Navigation

Context:  
A user enters their credentials using the phone keyboard and expects to submit the form without touching the screen again.

Source: End user.

Stimulus:  
The user presses the **Enter** key after typing the password.

Artifact: Login form.

Environment: Normal operation during form completion.

Response:  
The system initiates the login process immediately after the Enter key is pressed.

Metrics:

Task Completion: Do users successfully log in using only the keyboard?

Errors: Do they attempt to tap the login button because Enter does not trigger the action?

Efficiency: Time required to complete the login using keyboard interaction.

---

# 3. Attribute: Learnability

## Scenario: Login Flow Recognition

Context:  
A manual worker opens the application for the first time and wants to access his account.

Source: New user.

Stimulus:  
The user scans the screen looking for the action that allows them to log in.

Artifact: Login button and screen layout.

Environment: First-time use with no prior instructions.

Response:  
The login button is visually prominent and clearly labeled so users can identify it quickly.

Metrics:

Task Completion: Do users locate the login button without assistance?

Efficiency: Time required to identify the login action.

Errors: Do users attempt to tap other elements first?

---

## Scenario: Login Loading State Visibility

Context:  
A returning user attempts to log in while the server response is slightly delayed.

Source: Returning user.

Stimulus:  
The user presses the login button.

Artifact: Login button (loading state).

Environment: High network latency.

Response:  
The login button displays a loading indicator and becomes temporarily disabled to prevent duplicate requests.

Metrics:

Errors: Number of times users attempt to press the button repeatedly.

Awareness: Do users recognize that the system is processing their request?

---

## Scenario: Password Correction

Context:  
A user realizes they made a typing mistake while entering their password.

Source: End user.

Stimulus:  
The user deletes characters and retypes their password.

Artifact: Password input field.

Environment: Normal login interaction.

Response:  
The system allows users to edit the password field easily without clearing the entire form or losing the email field content.

Metrics:

Errors: Number of corrections made while typing the password.

Completion: Do users successfully correct their password and log in?

User Reaction: Do they appear confused while editing the password?

---

# 4. Attribute: Satisfaction

## Scenario: Session Persistence

Context:  
An employee opens the application again shortly after previously logging in.

Source: Returning user.

Stimulus:  
The user launches the application.

Artifact: Session management system.

Environment: Normal operation with a previously active session.

Response:  
The system keeps the user session active and opens the main screen without requiring another login.

Metrics:

Task Completion: Do users access the main interface without re-entering credentials?

User Reaction: Do users appear surprised or relieved that they do not have to log in again?

---

## Scenario: Interface Trust and Professional Appearance

Context:  
A new patient opens the application for the first time and evaluates whether the system looks trustworthy.

Source: New user.

Stimulus:  
Initial visualization of the login screen.

Artifact: Login interface design and branding.

Environment: First contact with the application.

Response:  
The interface presents a clean layout with clear institutional branding that communicates reliability and professionalism.

Metrics:

Perceived Trust: User rating of the interface's credibility.

Message Comprehension: Do users understand that this is the official medical system login?

---
