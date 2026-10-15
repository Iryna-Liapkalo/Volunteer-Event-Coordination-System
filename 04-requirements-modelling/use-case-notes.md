# Week 4 — Requirements Modelling: Use Case Diagram


## 1. Requirement Used
FR-01 (Account & Profile): The system shall allow volunteers to register an account and select their skills, general availability, and upload qualification documents
FR-03 (Automated Verification Check): The system shall automatically prevent unverified volunteers from registering for restricted roles requiring background checks e.g., Garda vetting
FR-05 (Roster Management): The system shall allow event organisers to view, confirm, and export volunteer attendance rosters for their assigned events



## 2. Requirement Analysis (Requirement -> Actor -> Goal -> Use Case)


### Analysis of FR-01:
1. Goal: Register as a volunteer, specify skills/availability, and provide credentials for role eligibility
2. Use Case Name: Register Profile & Qualifications
3. Actor Check: General Volunteer / Skilled Volunteer
4. Clarification Question: Can a volunteer browse events before completing their qualification uploads, or is profile completion mandatory at sign-up


### Analysis of FR-03:
1. Goal: Ensure only vetted volunteers are assigned to sensitive community roles e.g., working with youth or vulnerable adults
2. Use Case Name: Apply for Restricted Event Role
3. Actor Check: Skilled Volunteer (Primary) and Garda Vetting / Verification System Secondary/External Actor
4. Clarification Question: Does the system automatically query an external Garda vetting database, or does an admin manually check uploaded certificates



## 3. Actors
General Volunteer (Primary Actor): An external user who creates a profile, browses community events, and registers for basic volunteer tasks
Skilled Volunteer (Primary Actor): An external user with verified qualifications (e.g., Garda vetting, first aid) who applies for specialized roles
Event Organiser (Primary Actor): An external user responsible for creating events, managing volunteer rosters, and sending notices
Garda Vetting System (Secondary / External System Actor): An external system that provides qualification verification status



## 4. Use Cases (Inside System Boundary)
Register Profile & Qualifications
Browse Community Events
Apply for Restricted Event Role
Create & Manage Event
Export Volunteer Roster



## 5. Answers to Part 7: Modelling Problems Analysis

Example | What is wrong?  Corrective Action 

Database drawn as an actor. A database is an internal technical component, not an external user or external system. Remove Database; actors must be external entities e.g., Volunteer, External Verification API
Booking Screen drawn as a use case. A screen is a User Interface element, not a functional goal or behavior. Rename to a verb-goal phrase like Apply for Restricted Event Role
Volunteer placed inside boundary. An actor represents an external entity interacting with the system, so it must stay outside the boundary box.  Move the `Volunteer` actor outside the system boundary
Do Stuff used as a use case name. Too vague; does not describe a clear, meaningful user goal Use specific action verbs, e.g., Export Volunteer Roster
Every stakeholder added as an actor. Not all stakeholders directly interact with the software e.g., Community Sponsor or Privacy Office. Include only stakeholders who directly trigger or interact with use cases. 



## 6. Unknowns / Questions Raised by the Model
1. Verification Expiry: What happens when a volunteer’s Garda vetting status expires while they are already registered for an upcoming event
2. Roster Promotion: When a volunteer cancels their registration, does the system automatically promote the next person on the waitlist, or does the Event Organiser approve it manually



## 7. Reflection
What the diagram helped understand: It clearly defined the system boundary for the Community Volunteer & Event Coordination System* and separated standard volunteer goals from administrative organizer functions
Uncertainty revealed: The diagram highlighted an ambiguity regarding verification — specifically whether credential checks are performed real-time by an external API or asynchronously by an admin
