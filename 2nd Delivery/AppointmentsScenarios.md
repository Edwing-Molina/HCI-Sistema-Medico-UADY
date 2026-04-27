# Quality Attribute Scenarios for the Login Module

---

## 1. Attribute: Protection Against User Errors

*Focus: Robustness and proactive validation.*

| Scenario | 1.1 Format Validation | 1.2 Brute Force Prevention | 1.3 Empty Field Integrity | 1.4 Network Resilience |
| :--- | :--- | :--- | :--- | :--- |
| **Source** | End user | Attacker or confused user | End user | External environment (Network) |
| **Stimulus** | Entering an email without "@" or with invalid characters | 5 failed login attempts within 60 seconds | Clicking the "Login" button with empty fields | Loss of connection during the login request |
| **Artifact** | Login Form (TextFormField) | Authentication API / Backend | Primary Action Button | Communication layer (HTTP Client) |
| **Environment** | Normal operation | Normal operation | Normal operation | Low connectivity or micro interruptions |
| **Response** | The system immediately shows a visual error message and blocks submission | The system temporarily locks the account and returns to the login page | The button remains disabled or highlights missing fields in red | The system shows a friendly timeout message and allows retry without clearing data |
| **Measure** | **100%** of syntax errors blocked before reaching the API | Lock activated after the 5th attempt; response time < **1s** | **EPE (Error Prevention Effectiveness)** of **100%** | **100%** data persistence after network recovery |

---

## 2. Attribute: Accessibility

*Focus: Inclusion of patients and beneficiaries with disabilities (WCAG 2.1).*

| Scenario | 2.1 Interface Scaling | 2.2 Non-Visual Perception | 2.3 Motor Precision |
| :--- | :--- | :--- | :--- |
| **Source** | Elderly user | User with color blindness | User with reduced mobility |
| **Stimulus** | System font increased to **200%** | Appearance of a validation error | Attempt to tap the information links |
| **Artifact** | Screen layout (Scaffold/Column) | Error messages and alerts | Interactive elements (Buttons/Links) |
| **Environment** | Assistive technology in use | Customized OS configuration | Normal operation | Normal operation |
| **Response** | Layout adapts with scrolling without overlapping or cutting text | The system uses warning icons in addition to red color to signal failure | The system registers touches due to sufficiently large touch areas |
| **Measure** | **0%** pixel overflow on screen | **100%** of errors understandable without relying on color | Minimum touch area of **44x44 dp** for all elements |

---

## 3. Attribute: Intuitiveness

*Focus: Ease of learning and use without training.*

| Scenario | 3.1 Flow Recognition | 3.2 State Visibility | 3.3 Control Consistency |
| :--- | :--- | :--- | :--- |
| **Source** | New user | Returning user | End user |
| **Stimulus** | First attempt to access the application | Long server response time | Attempt to view the typed password |
| **Artifact** | Visual hierarchy of the screen | Login Button (Loading State) | Letters showed for a moment when user writes in password field |
| **Environment** | First-time use (no manual) | High network latency | Normal operation |
| **Response** | The user identifies the login button as the most prominent element on the screen | The button shows a loading indicator and becomes non-interactive | The character state reveals the text immediately for a moment |
| **Measure** | **90%** of users log in within **<20s** without assistance | **0** duplicate clicks recorded during waiting | User reaction time to identify what are typing for < **2s** |

---

## 4. Attribute: Satisfaction

*Focus: Trust and perceived service quality.*

| Scenario | 4.1 Biometric Agility | 4.2 Institutional Trust |
| :--- | :--- | :--- |
| **Source** | Returning user | New user |
| **Stimulus** | Opening the application with a previous session | Initial visualization of branding and design |
| **Artifact** | Local authentication module | Visual aesthetics and Login UI |
| **Environment** | Daily use | Normal operation |
| **Response** | The system automatically use cache of the app to avoid manual typing login | The user perceives a clean, professional interface with clear medical branding |
| **Measure** | **80%** reduction in access time (vs manual login) | Perceived satisfaction score > **4.5/5** in surveys |

---
