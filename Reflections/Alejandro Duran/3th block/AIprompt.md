# Reflection: AI as the Architect of Our Testing Protocol Plan

**Core Idea: AI can transform the way testing protocols are built by enabling comprehensive, structured, and scalable design—provided it is guided by clear human intent and well-defined quality attributes.**

## Reflection

**Claim (Main Argument):**  
Using AI to build the entire testing plan, using scenarios to writing the full usability testing protocol—felt like shifting from manual construction to using automatic tool. It allowed us to cover five quality attributes (Usability, Accessibility, Efficiency, Learnability, and Reliability) simultaneously, something that would have taken days to organize manually without missing important details.

**Data (Evidence):**  
If done manually, designing scenarios for five different attributes would have required hours of discussion just to decide what to test. Instead, we used a **chained prompt approach**: first generating scenarios, then using those as the foundation for the full testing protocol.  
What would normally take days of meetings was reduced to a single afternoon of refining prompts. Around **90% of the heavy drafting work** was completed by AI in seconds, leaving the team to focus only on adjustments and validation.

**Warrant (Reasoning):**  
The effectiveness of this process lies in the **connection between prompts and outputs**. By explicitly defining the five quality attributes, the AI was able to generate a protocol that evaluates not only usability cases, but also deeper aspects like efficiency and accessibility . In this sense, the prompt acts as a translator and more complete about all the needing of the program, turning abstract concepts into testing instructions.

**Backing (Additional Support):**  
One major advantage of using AI is **consistency**. Human-written protocols often vary in depth and quality across sections, but AI maintained a uniform level of rigor across all five attributes. Additionally, it helped ensure that the testing language remained neutral, avoiding unintentional bias or guidance that could influence user behavior during testing.

**Qualifier (Limitations):**  
This approach only works effectively if the inputs are well-defined. Without clearly specifying the five quality attributes from the start, the AI would produce a generic and less useful protocol. The tool is powerful, but it depends entirely on the clarity and direction provided by the team.

**Rebuttal (Counterargument):**  
Some may argue that automating protocol creation removes the “human element” from usability testing. However, the opposite can be true: by delegating the documentation and structuring tasks to AI, the team gains more time to focus on observing real users, understanding their struggles, and interpreting their emotions—arguably the most human part of the process.

## Team Project Example: Medical Services App

In our project, we implemented a **chained prompt workflow**:

1. **Scenario generation:**  
   We asked AI to create realistic and challenging situations for each of the five attributes (Usability, Accessibility, Efficiency, Learnability, Reliability).  
   For example: *“A user that needs to book an urgent appointment in low-light conditions and has forgotten her glasses.”* This scenario simultaneously evaluates accessibility and efficiency.

2. **Protocol generation:**  
   Using those scenarios, we prompted the AI to build a complete usability testing protocol, including facilitator instructions, user tasks, and measurable metrics.

As a result, our testing plan went beyond simple step-by-step instructions. It evaluated whether our user could:
- Complete a task within a specific time frame (Efficiency),  
- Understand icons without reading labels (Learnability),  
- Successfully navigate under constrained conditions (Accessibility).  

This approach gave us a **holistic testing framework** that covered multiple angles at once—something that would have been difficult and time-consuming to achieve manually.

Ultimately, the AI-generated protocol served as a structured foundation, while the team ensured its relevance and alignment with the real context of a UADY medical services application.

---

## References

- Human-Computer Interaction (HCI) principles on usability and testing  
- Interaction Design Foundation (iXDF) guidelines  
- Project experience using AI for scenario and protocol generation
