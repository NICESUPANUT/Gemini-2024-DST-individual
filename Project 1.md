# Observe Science Plan

## Use Case ID: UC001
**Importance Level:** Medium  
**Primary Actor:** Science Observer  
**Use Case Type:** Detail, Essential  

## Stakeholders and Interests
1. **Science Observer** - Ability to edit or correct errors directly.
2. **System** - Accurately displays science plan details, tracks, and updates the status of science plans and observations.

## Brief Description
Science Observer observes the science plans submitted by astronomers into the system.

## Trigger
Science Observer wants to observe the science plan.

## Type
User-Driven Process

## Relationships
- **Association:** Science Observer, System
- **Include:** Transform Science Plan to Observing Program
- **Extend:** None
- **Generalization:** None

---

## Normal Flow of Events
1. The Science Observer selects a Science Plan to review.
2. The System displays the details of the selected science plan.
3. The Science Observer reviews the science plan for accuracy.
4. The Science Observer confirms the observation or requests further actions.
5. The System records the observation status and updates the plan accordingly.

---

## Subflows
### (3a) Viewing Additional Science Data
- The observer wants to see more detailed data (e.g., historical observations).
- **System Response:**
  - Retrieves and displays the requested data.
  - The observer can continue the review with this additional context.

### (3b) Handling Data Errors in Science Plan
- The observer reviews the science plan details and detects incomplete or incorrect data.
- **System Response:**
  - Highlights missing or invalid fields.
  - Allows the observer to edit and correct the data directly.
  - Saves changes and returns to the review step.

### (4a) Observation Cancellation
- The observer confirms or cancels the observation.
- **System Response:**
  - Saves any changes as a draft.
  - Allows the observer to resume later without losing progress.

---

## Alternate/Exceptional Flow
### (2a) Science Plan Not Found
- When the system attempts to display the science plan but it is deleted or unavailable.
- **System Response:**
  - Shows an error message: `"Science Plan not found."`
  - Redirects the observer to the selection screen.

### (5a) System Crash
- When the system records the observation status but crashes.
- **System Response:**
  - Auto-saves observation progress.
  - Notifies the observer and allows them to resume when the system recovers.

---

## Diagrams
![Activity Diagram](![image](https://github.com/user-attachments/assets/0c38112a-01d3-4a0f-b6a6-9bc9afe917e4)  
![Sequence Diagram](![image](https://github.com/user-attachments/assets/0a98c854-6d44-4f46-b3cd-6d3628bebfdb)


| **Use Case Name:** transform Science Plan to Observing Program | **ID:** UC002 | **Importance Level:** High |
|--------------------------------------|------|------------------|
| **Primary Actor:** Science Observer | **Use Case Type:** User-driven |

## **Stakeholders and Interests**
- **Science Observer:** Needs to accurately transform a Science Plan into an Observing Program to ensure correct execution  
- **Astronomer:** Depends on the transformation process to ensure the proposed observations are correctly scheduled  
- **Telescope Operator:** Uses the Observing Program to control the telescope and execute the observations  
- **Observatory System:** Stores and processes the transformed Observing Program for scheduling and execution  

## **Brief Description**
This use case describes how a **Science Observer** takes an approved **Science Plan** and transforms it into an **Observing Program**, ensuring it is correctly formatted and contains all necessary parameters for execution by the observatory system.  

## **Trigger**
- **Science Plan** is approved and submitted to the system.  

## **Type**
- User-Initiated  

## **Relationships**
- **Association:** Science Observer  
- **Include:** -  
- **Extend:** -  
- **Generalization:** -  

## **Normal Flow of Events**
1. The Science Observer retrieves an approved Science Plan from the system  
2. The system provides the necessary observation parameters  
3. The Science Observer verifies and adjusts observation parameters if needed  
4. The Science Observer converts the Science Plan into an Observing Program format  
5. The system validates the transformed Observing Program for completeness and correctness  
6. If validation is successful, the Science Observer submits the Observing Program to the system  

## **Subflows**
- If the Science Plan contains errors or missing information, the Science Observer requests corrections  
- The Science Observer may consult with the Astronomer to clarify scientific objectives  

## **Alternate/Exceptional Flow**
- If the system detects missing data in the Observing Program, it notifies the Science Observer for revision  
- If there is a technical issue with system validation, the Science Observer reports it to system support  

## **Activity Diagram**
![image](https://github.com/user-attachments/assets/76968ced-eea2-4a79-acb3-bf80297b0692)

## **Sequence Diagrams**  

![image](https://github.com/user-attachments/assets/60fd49ee-4436-4341-8bc4-0d146be89025)



