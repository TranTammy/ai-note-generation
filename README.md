# ai-note-generation
SE 4485.001 Software Engineering Project sponsored by ARGO

This project will create a service that utilizes an existing BHCC Simulator Application, adding an AI feature to generate notes for patients' medical records. A dedicated Note Generation Service that handles all note-related logic will also be created. This service will also expose a RESTful API that allows both manual and automated requests.

<ins>**Project Overview:**<ins>

**Background**

A simple user interface (UI) has already been built to interact with these APIs. The UI allows a user to select a mock
patient, choose a note type (category) and sub-category, manually add a note, and then submit a request.
• Note generation API Endpoints: Our existing service provides endpoints for creating different types of notes.
These endpoints accept patient identifiers and note-specific parameters.
• Patient Data Access API Endpoints: These endpoints, also provided by BHCC, allow retrieval of mock patient
data which includes all available notes. This allows the Note Generation service to have context on previously
submitted notes.

**Objective #1**

To integrate an AI tool using the Note Generation Service as a middleware. Instead of having a user type the entire note, the
UI would capture a few key inputs from the user, such as the patient's current state, the type of note needed, and a high-level
summary of the "patient journey" flow.

**Objective #2**

Develop an automated note creation feature that can be built on top of the existing (Objective #1) architecture without
significant changes to the core logic. This can later be discussed on how often the scheduled job runs, and other details.

<ins>**Configuration Management (CM) Details:**<ins>

1. Follow kebab case/dash case for all file naming convention.
2. Before committing changes to documents/files, at least two peer reviews must take place.
3. Attach appropriate description that "gives information that helps the understanding of each change."
