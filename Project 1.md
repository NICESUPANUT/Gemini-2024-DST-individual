## **Class Diagram**
![image](https://github.com/user-attachments/assets/ac699d76-97f4-481a-b3d7-0e6b42bff80e)


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



