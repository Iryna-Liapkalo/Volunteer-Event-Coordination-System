# Week 5 — Activity Diagram Modelling

## 1. Purpose
This activity diagram models the process of a volunteer submitting an application for an event role in the Community Volunteer & Event Coordination System.
It shows the main activities and the decision point related to Garda Vetting status.

## 2. Process Description
The process begins when a volunteer selects an event role. The system checks the volunteer’s Garda Vetting status
A decision is then made based on whether the status is valid:
Valid: The volunteer can continue and submit an application. The system records the application
Invalid: The process leads to an unknown outcome because the system’s behaviour in this situation has not yet been confirmed.
The process ends after the application has been recorded.

## 3. Main Activities
1. Select Event Role.
2. Check Garda Vetting Status.
3. Decide whether Garda Vetting is valid
4. If valid, submit the application
5. Record the application.
6. End the process

## 4. Decision and Open Questions
The decision point is Is Garda Vetting valid
The diagram includes two possible paths:
Valid: Continue to application submission.
Invalid: The outcome is currently unknown.
Further stakeholder clarification is needed to establish what should happen when Garda Vetting is invalid, expired, missing or pending
The system should not automatically approve or reject an application unless this behaviour is confirmed by stakeholders.

## 5. UML Notation
The diagram uses standard UML Activity Diagram elements
Filled circle — initial node
Rounded rectangles — activities
Arrows — control flow.
Diamond — decision point.
Branch labels — valid and invalid paths
Final node — end of the process

## 6. Reflection
Creating this activity diagram helped me understand the sequence of actions involved in submitting an application. It also highlighted an unresolved business rule concerning Garda Vetting.
The diagram separates application submission from approval. Further stakeholder input is required before defining the behaviour for invalid or unconfirmed Garda Vetting statuses
