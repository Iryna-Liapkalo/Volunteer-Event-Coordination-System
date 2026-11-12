# Week 4 — Requirements Modelling: Use Case Diagram

## 1. Requirements Selected
The use case diagram is based on the Community Volunteer & Event Coordination System
The main requirements are:
FR01: Volunteers can create an account.
FR02: Volunteers can manage their profile, skills and availability
FR04: Authorised organisers can create and manage events and roles
FR05: The system restricts applications for designated roles based on verified qualifications.
FR08 Candidate: Volunteers can submit applications for available event roles. This requirement needs stakeholder confirmation

## 2. Actors
Actor | Description 
Volunteer | Registers, manages a profile, browses events and applies for roles. 
Event Organiser | Creates and manages events and volunteer roles. 

A Privacy / Compliance Officer is a stakeholder but is not currently shown as an actor because direct interaction with the system has not been confirmed.

## 3. Main Use Cases
Use Case | Actor | Requirement 
Register Account | Volunteer | FR01 
Maintain Volunteer Profile | Volunteer | FR02 
Browse Events and Roles | Volunteer | Candidate 
Submit Application for Event Role | Volunteer | FR08 
Create and Manage Events and Roles | Event Organiser | FR04 

## 4. System Boundary
The system boundary is labelled community Volunteer & Event Coordination System
Actors are placed outside the boundary, while use cases are placed inside it. Association lines show which actors interact with each use case.
No include or extend relationships are used because they are not necessary for this initial model.

## 5. Open Questions

1. Can volunteers browse restricted roles before their qualifications are verified
2. Is qualification verification performed manually or through an external system
3. Can volunteers apply for multiple roles within the same event?
4. Should event creation and role management be separate functions?

These questions require clarification from the Event Organiser and Privacy / Compliance Officer.

## 6. Conclusion
This week helped me understand how Use Case Diagrams represent interactions between actors and a system. I identified the main actors, their goals and the system boundary.
I also learned that use cases should describe meaningful user goals rather than individual screens or database operations. The diagram provides a clear overview of the system's functional requirements and highlights areas that need further stakeholder clarification.
