# Project Plan - UADY Medical Service App

## Application Objective

The main objective of the application is to simplify and digitize the procedures 
that beneficiaries of the Medical Service at the UADY currently perform in 
person at the service window or by phone.

The goal is to develop an inclusive mobile tool that allows all beneficiaries 
—regardless of their level of technological experience— to schedule medical 
appointments, manage medical passes, consult their medical records, and handle 
procedures for their dependents (children and spouses) in an autonomous, secure, 
and efficient manner.

The application is designed under a User-Centered Design (UCD) approach, 
prioritizing accessibility and usability for two contrasting profiles: manual 
labor workers (janitors, maintenance staff) with significant technological 
barriers, and faculty/administrative staff (ages 45-70) with needs for 
legibility and clear navigation. This dual approach aims to bridge the digital 
gap between manual and digital processes for all levels of the university 
community.

---

## Project Plan

### Research Plan

The research will focus on understanding the needs, behaviors, frustrations, 
and technological proficiency of the beneficiaries of the UADY Medical Service. 
Information will be gathered through field observation at the Medical Service 
window, contextual interviews with workers of different profiles (manual labor, 
faculty, and administrative staff) conducted at their workplaces, and a digital 
survey on technological profile distributed to the university community. Data 
analysis will be performed using qualitative and quantitative methods following 
the Nielsen and Ramdhani methodology for Persona construction. This includes:

- **Definition of required information:** Current Medical Service processes 
  (appointment scheduling, pass management, record consultation) will be 
  analyzed to identify friction points, access barriers, and unmet needs of 
  beneficiaries. The research seeks to answer key questions such as: How do 
  they currently perform their procedures? What technological barriers do they 
  face? What level of digital experience do they have? What functionalities 
  would they prioritize in an app?

- **Instrument creation:** Three main instruments will be designed:
  1. **Field observation guide** to document real behaviors at the Medical 
     Service window (wait times, interactions, visible frustrations).
  2. **Semi-structured interview guide** with 20 questions organized in 
     4 blocks (general data, Medical Service experience, technological 
     profile, and app expectations).
  3. **Digital technological profile survey** 
     with 17 questions to quantify the level of digital experience, technology 
     usage habits, and expectations of beneficiaries.

- **Type of analysis:** Thematic analysis (open coding) will be applied to 
  interviews and observation notes, identifying behavioral patterns and need 
  categories. For surveys, descriptive statistics will be used to profile the 
  average technological level of users. Results will directly feed the 
  refinement of Personas, Usage Scenarios, and the validation of Functional 
  and Non-Functional Requirements.

---

### Activity Schedule

| Date | Activity | Observations | Resulting Product |
|------|----------|--------------|-------------------|
| 02/17/26 | Project scope and objectives definition | The team will meet to define the system's objective, identify the main stakeholders, and establish the dual approach (manual labor users vs. faculty/administrative staff). The use of the UCD methodology and Nielsen/Ramdhani as a theoretical framework will be determined. | Application definition document (objective, motivation, relevance, stakeholders) |
| 02/18/26 | Stakeholder analysis and Persona creation | The stakeholder analysis (primary and secondary) will be formalized and 3 Personas will be constructed based on the Nielsen and Ramdhani methodology: Don José (manual labor worker, primary persona), Dra. Elena (senior faculty, secondary persona), and Mariana (young administrative staff, tertiary persona). Each persona will include demographics, technological profile, goals, frustrations, and design impact. | Stakeholder document and Personas with formal structure |
| 02/19/26 | Requirements definition | User Requirements (UR), Functional Requirements (FR01-FR16), and Non-Functional Usability and Accessibility Requirements (NFR-U-01 to NFR-U-07) will be defined based on the initial stakeholder analysis and the Medical Service context. Type distinction and connection with user profiles will be established. | Requirements document (UR + FR + NFR) in MD and bilingual PDF format (ES/EN) |
| 02/19/26 | Usage scenarios creation | Three narrative usage scenarios will be developed connecting Personas with Functional Requirements: (1) Don José schedules an appointment for his daughter, (2) Dra. Elena manages her husband's medical pass, (3) Mariana cancels and reschedules an appointment quickly. Each scenario will include context, step-by-step flow, involved requirements, and critical usability points. | Usage scenarios document |
| 02/20/26 | Similar systems review (Benchmarking) | At least 5 similar systems will be analyzed (IMSS Digital, ISSSTE Citas, Doctoralia, MyChart, Mi Salud) evaluating their strengths, weaknesses, and lessons applicable to the project. Innovation elements that differentiate our proposal will be documented. | Benchmarking and innovation analysis document |
| 02/20/26 | Research instrument design | The 3 instruments for the data collection phase will be created: field observation guide, semi-structured interview guide, and digital technological profile survey. An internal review will be conducted to validate that the questions cover all aspects necessary to refine Personas and validate requirements. | Observation guide, interview guide, digital survey (Forms), informed consent form |
| 02/21/26 | UCD Methodology documentation | A document will be written describing how the User-Centered Design methodology (ISO 9241-210) is applied in the project, mapping UCD phases to the course deliverables and justifying the choice of research methods. | UCD methodology document |
| 02/22/26 | Repository organization | The GitHub repository will be restructured with the final folder structure, naming conventions, updated .gitignore, and main README with the complete project description. Issues, Milestones will be configured, and all members' contributions will be verified. | Organized and documented repository |
| 02/23/26 | Individual reflections | Each team member will write their personal reflection on the work process, learnings, and contributions in the first delivery. | Individual reflections (1 per member) |
| 02/24/26 - 02/25/26 | Integration, final review, and presentation preparation | All artifacts will be integrated into the delivery folder, a cross-review of all documents will be performed, consistency between documents will be verified (stakeholders ↔ personas ↔ scenarios ↔ requirements), and the progress presentation will be prepared. | Complete Delivery 1, presentation slides |
| **02/26/26** | **🎯 DELIVERY 1 DEADLINE** | **Final submission of all artifacts and presentation of progress to the professor.** | **Complete Delivery 1 package** |

---

### Roles and Responsibilities

- **Edwing Molina Chim:** Project Lead & Repository Manager. Responsible for 
  the structure and organization of the GitHub repository, definition of 
  non-functional usability and accessibility requirements, integration of 
  documents from all areas, overall team coordination, and ensuring 
  consistency between deliverables.

- **Alejandro Magdiel Durán Varela:** Requirements Engineer. Responsible 
  for the definition and formal documentation of User Requirements, 
  Functional Requirements (FR01-FR16), and their connection with stakeholder 
  needs. In charge of generating professional PDF documents and bilingual 
  versions (Spanish/English) of the requirements.

- **Lexus Harit Parra Kauil:** UX Researcher. Responsible for research plan design, the creation of Personas and Usage Scenarios based on the Nielsen and Ramdhani methodology, and the benchmarking analysis of similar systems.

- **Jesús Everardo Jiménez Rivera:** UX Analyst & Documentation Specialist. In charge of defining User Research activities, designing data collection instruments (interview guides, observation guides, and surveys), and conducting stakeholder analysis. Also responsible for documentation of the UCD methodology, support in document translation, and cross-review and validation of deliverables.

---

### Document Repository

To ensure the organization, traceability, and access to all project 
documentation, a digital repository has been established on GitHub:

🔗 **[HCI-Sistema-Medico-UADY](https://github.com/Edwing-Molina/HCI-Sistema-Medico-UADY)**

This repository will store:

- **Planning documents:** Research plan, activity schedule, roles and 
  responsibilities, and UCD methodology.
- **User research:** Stakeholder analysis, Personas, Usage Scenarios, 
  benchmarking of similar systems.
- **Data collection instruments:** Observation guides, interview guides, 
  surveys, and informed consent forms.
- **Requirements definition:** User, Functional, and Non-Functional 
  Requirements in MD, PDF, and bilingual formats.
- **Research results:** Observation notes, interview transcriptions, data 
  analysis, and key findings (future deliveries).
- **Design:** Wireframes, mockups, prototypes, and design system (future 
  deliveries).
- **Evaluation:** Heuristic evaluation and usability testing reports 
  (future deliveries).
- **Individual reflections:** Each team member's reflections per delivery.