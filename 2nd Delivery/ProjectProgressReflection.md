# Project progress


## Initial state prior to the first delivery

- The UADY medical service app project did not have a requirements specification document listing the functional and non-functional requirements; it only has user stories located in the Jira tool.
<img src= "/Assets/HU.png">
<br>
- The app is aimed at a general audience of UADY personnel, and there was no information available to create a UI design that meets user needs and ensures optimal experience and usage, as many decisions—such as using Microsoft 365 as the login method—cannot be changed; furthermore, the user interfaces were created to be very general and could be difficult to use for various groups of people.

<grid col= 2 pd= 5 w=250> 
    <img src="/Assets/Appointments.png"width="250" >
    <img src="/Assets/Login.png" width="250">
</grid>

<br>
<br>

- There is a design guide that focuses only on the look and feel of the application, supported by the [Manual de identidad UADY]("https://drive.google.com/file/d/10oMLtJlbZ_k_ifx5R4J2q7F5KzJBZwn8/view") for certain aspects the application must have, such as typography, UADY logo placement, and colors.
<br>
- We have a nearly finished app

## Our team's contribution

- As there was no SRS (Software Requirements Specification), a version was created where user stories were analyzed and synthesized for the functions that we, as a team, considered users would have the most trouble using, and the SRS was created with the functional and non-functional requirements.
[ERS]("/1st%Delivery/Requeriments.md")
<br>

- As there was no clear identification of the target audience, we decided to focus on those we considered to be the users who could have the most problems using the system, and we generated synthetic [Personas](/1st%20Delivery/Personas.md) with AI, with which we can identify these problems and the usability attributes that will help us know what to measure and what should interest us about the users to perform the usability tests (this applies only in our case because we are not going to create prototypes for the tests since the app already exists), which will help us later with a proposal where everything we have applied regarding User-Centered Design techniques will be reflected
<br>
- Surveys were conducted to gain deeper insights into the users participating in the usability testing, specifically focusing on their level of technical proficiency and other relevant considerations.
[Technological Profile](/1st%Delivery/User%Research/Instruments/Encuesta%perfil%tecnologico.md) - [Interview Guide](/1st%20Delivery/User%20Research/Instruments/Guia%20de%20entrevista%20semi-estructurada.md)
<br>
- Since there were no established standards or design guidelines for our user interfaces, we researched and implemented industry-leading usability standards. These included **WCAG 2.1 (Web Content Accessibility Guidelines)**, the global standard for accessibility, as well as the **Apple Human Interface Guidelines and Google Material Design** the definitive frameworks for iOS and Android development. By leveraging these standards, we defined our non-functional requirements focused on usability:

#### References and Usability Standards

##### 1. International Accessibility Standards
* **WCAG 2.1 (Web Content Accessibility Guidelines):** Compliance level **AA** was applied to ensure a contrast ratio of at least 4.5:1. This ensures readability for faculty and administrative staff between the ages of 45 and 70 who may experience visual fatigue or presbyopia.
    * *Source:* [W3C - Web Content Accessibility Guidelines 2.1](https://www.w3.org/TR/WCAG21/)


##### 2. Human Interface Guidelines (Tactile Ergonomics)
* **Apple Human Interface Guidelines & Google Material Design:** A recommendation for minimum touch targets of **44x44 dp/pt** was adopted. This is critical for "Manual Users" (Janitors/Maintenance) to facilitate interaction despite potential lack of digital experience or physical fatigue.
    * *Sources:* * [Apple Human Interface Guidelines - Accessibility](https://developer.apple.com/design/human-interface-guidelines/foundations/accessibility/)
        * [Material Design - Accessible Design](https://m3.material.io/foundations/accessible-design/overview)

##### 3. Heuristic Usability Principles
* **Jakob Nielsen's 10 Usability Heuristics:** Principles such as *Visibility of system status* (visual feedback) and the *Use of simple language* were applied to avoid technical jargon. This prevents excluding vulnerable populations during the digitalization process, such as those without institutional email accounts.
    * *Source:* [Nielsen Norman Group - 10 Usability Heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/)


