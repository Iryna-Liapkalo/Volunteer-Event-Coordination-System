# Week 4 — Requirements Modelling: Use Case Diagram

## 1. Requirements Selected
The use case diagram is based on the Community Volunteer & Event Coordination System
The main requirements are:
FR01: The system shall allow a volunteer to create an account.
FR02: The system shall allow a registered volunteer to record and update their skills and availability.
FR04: The system shall allow an authorised organiser to create, edit and cancel events and volunteer roles.
FR05: The system shall restrict applications for designated roles to volunteers whose required qualifications are recorded as verified.
FR08 (candidate): The system shall allow a volunteer to submit an application for an event role. This needs stakeholder confirmation.

## 2. Actors
The diagram shows three actors. Their names are generic and I have mapped them to the scenario below.

Actor in diagram | Mapped to scenario | Status 

User | Volunteer | Supported: volunteers register, browse events and apply. 
Administrator | Event Organiser (event management); possibly IT Support / System Administrator (user management) | Partly supported. Needs clarification (see Open Questions 1 and 2). 
Reviewer | Unknown role (possibly an organiser reviewing applications or someone verifying qualifications) | Not confirmed. The scenario does not state who reviews or verifies. 

A Privacy / Compliance Officer is a stakeholder but is not shown as an actor because direct interaction with the system has not been confirmed.

## 3. Use Cases
Use case in diagram | Actor | Requirement / evidence | Status 

Signup | User (Volunteer) | FR01 | Supported |
Browse Events | User (Volunteer) | Candidate (viewing upcoming events) | Candidate 
Register for Events | User (Volunteer) | FR08 (application for an event role) | Candidate 
Manage Events | Administrator (Event Organiser) | FR04 | Supported 
Login | User, Administrator | No requirement yet | Not confirmed (see Q3) 
Submit Material | User (Volunteer) | Possibly qualification evidence (FR03) | Not confirmed, needs clarification 
Manage Users | Administrator | No requirement yet | Not confirmed 
Manage Submissions | Administrator | No requirement yet | Not confirmed 
Review Submissions | Reviewer | Possibly verification linked to FR05 | Not confirmed 

FR02 (maintain profile) and FR05 (restriction by verified qualifications) are listed in Section 1, but the diagram has no separate use case for them. FR02 is not shown and FR05 may relate to Review Submissions. These are gaps found by the model.


## 5. Open Questions
1. Is the Administrator the same person as the Event Organiser, or are these different roles (for example, IT Support managing users)?
2. Who manages user accounts, and is "Manage Users" needed at all?
3. Is a separate Login use case required, or is login part of other functions?
4. What are "Submit Material", "Manage Submissions" and "Review Submissions" in this scenario? Do they mean qualification evidence and application review?
5. Who is the Reviewer and who verifies volunteer qualifications?
6. Can volunteers browse restricted roles before their qualifications are verified?
7. Can volunteers apply for multiple roles within the same event?
8. Should event creation and role management be separate functions?

These questions need clarification from the Event Organiser and the Privacy / Compliance Officer.

## 6. Reflection What the diagram helped me understand: the main goals of the volunteer (sign up, browse events, apply) and of the organiser (manage events), and that use cases should describe goals rather than screens or database operations.
