# Week 5 — Activity Diagram

## 1. Process Modelled
Apply for Restricted Event Role (Community Volunteer & Event Coordination System)

## 2. Purpose
To model the step-by-step workflow and operational control flow for the Apply for Restricted Event Role use case. The activity diagram helps clarify process sequences, identify decision logic, expose missing business rules, and communicate requirements clearly with stakeholders.

## 3. Activities
1. Select Restricted Event Role
2. Check Garda Vetting Status
3. Submit Application
4. Application Recorded

## 4. Decision and Guards
Decision Node: Is Garda vetting status valid?
Guards:
[valid]— Proceeds to Submit Application
[invalid / expired / missed] — Diverts to UNKNOWN Note

## 5. Unknowns
The system logic is unclear regarding how to handle applications when a volunteer's Garda vetting is currently pending, expired, or missing in the database.

## 6. Stakeholder Question
Should volunteers with pending or expiring Garda vetting be allowed to submit a conditional application, or must vetting be 100% active prior to application?


## 7. Modelling Decision
Adhered strictly to the UML 2.5 core notation rules provided in the practical guidelines:
Used an Initial Node (solid black circle) to mark the process start.
Used rounded rectangles for verb-based actions Select Restricted Event Role, Check Garda Vetting Status
Avoided introducing unsupported logic such as automated re-verification requests or instant rejection workflows without stakeholder validation.
Represented ambiguity explicitly using an UNKNOWN note rather than guessing business behavior.
Concluded successful paths with a Final Node bullseye symbol

## 8. Reflection
* **Process Clarity:** Transitioning from a Use Case ("WHAT goal") to an Activity Diagram ("WHAT HAPPENS step-by-step") exposed procedural logic and exact decision gates.
* **Exposing Assumptions:** The exercise demonstrated how activity modelling naturally highlights missing business rules (e.g., handling vetting exceptions), preventing developers from making unverified assumptions.
