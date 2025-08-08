Title: Generate BA User Story from Requirements Doc
role: BA
tags: [ui-requirements, user-story, acceptance-criteria, user-flow, definition-of-done]
version: 1.0
last_updated: 2025-08-08
author: akshata.parab
---
 
# 🧬 Generate BA User Story from Requirements Doc
 
## 🧩 Use-case
Business Analyst needs to convert a feature document into a UI-focused user story with compliance and accessibility details.
 
## 🧠 Prompt

You are provided a feature/requirements document (DOCX, TXT, etc.). Provide the output int he MD file only.
 
From a **Business Analyst perspective** in the **Payments domain**, complete the following. Ensure the output supports **UI clarity**, **developer/tester usability**, and meets **security & compliance** (e.g., PCI-DSS, GDPR) expectations.
 
**Step 1 – Convert to Markdown (.md)**  
Use clear headings, bullet points, and sections.
 
**Step 2 – Extract only UI-related requirements**  
Focus on inputs, layout, buttons, validation, interactions, and visual behaviors.
 
**Step 3 – Create a UI User Story**  
- Based on the **Who / What / Why** model  
- Follows **INVEST** principles  
- Includes **security**, **compliance**, and **accessibility** notes  
- Developer- and tester-friendly  
- Format in **Markdown**
 
---
 
**Output Format:**
 
UI User Story – [Feature Name]  
**Epic:** [Epic Name]  
**Module:** [Screen/Flow]  
**Platform:** [Web / Mobile / Tablet]
 
---
 
### User Story  
**As a** [user],  
**I want to** [goal/action],  
**So that** [business value].
 
---
 
### Acceptance Criteria  
1. [Field validation / behavior]  
2. [Security or masking rules]  
3. [Responsive layout or layout switching]  
4. [Error and success messaging behavior]  
5. [Compliance and audit logging requirements]  
6. [User flow or journey: describe steps the user follows through the UI]  
7. [Consent, opt-in/out, or privacy notice handling if applicable]  
8. [Accessibility compliance – WCAG 2.1 AA]
 
---
 
### UI Elements  
**Fields, Buttons, Icons** – labels, types, rules  
**Messages** – inline/global, duration  
**Conditional logic** – visibility or auto-fill
 
---
 
### Behavior & Layout  
- Layout expectations  
- Default values  
- Interaction flow  
- Accessibility (e.g., WCAG focus state, screen readers)
 
---
 
### Dependencies & Assumptions  
- APIs/services  
- Pending design decisions  
- Auth, privacy, audit needs
 
---
 
### Definition of Done  
- All Acceptance Criteria are met  
- UI matches design mockups across supported platforms  
- Validations work as specified (client + server)  
- All actions are logged per compliance standards  
- Screens are responsive and WCAG 2.1 AA compliant  
- Successful handoff to QA with test scenarios mapped to criteria  
- Stakeholder sign-off received for functionality and UI
 
First convert to Markdown, then generate the structured user story accordingly.
 (See <attachments> above for file contents. You may not need to search or read the file again.)
