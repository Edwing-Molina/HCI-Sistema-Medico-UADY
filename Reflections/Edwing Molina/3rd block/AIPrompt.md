# AI Prompt Reflection

In our case, we use AI almost 100% of the time to streamline our document creation processes. Initially, we faced some challenges because the AI wasn't delivering the results we wanted. To fix this, we first focused on creating quality scenarios; we used these as a foundation to then ask the AI for a testing protocol and evaluate its initial output.

During the creation of these quality scenarios, we provided the AI with:

- Synthetic personas created using the "Personas" technique.

- The attributes we intended to measure.

- Basic metrics that helped us ensure those attributes were covered.

From there, we began shaping the scenarios by providing mocks, application screenshots, and details on the specific modules to be tested. The first versions it produced were quite good, though it occasionally generated scenarios that were completely irrelevant. To refine this, we asked it to generate 10 to 15 scenarios per attribute for each module. We then reviewed and modified the ones we felt were most effective for measuring and guiding our tests.

Once the scenarios were ready, we asked Gemini to generate the testing protocol using the following prompt:

"Based on the following scenarios, provide the testing protocol. Keep our target audience in mind. Note that the scenarios provided below are specifically for the Appointment Scheduling module: [Scenarios]"

We iterated by comparing the AI's output against our app's prepared flow—considering both standard flows and exceptions—to create the tasks and all other protocol components. After a few instructions asking the AI to check for missing elements and add tasks to the testing flow, we reached the best version of our semi-formal protocol.