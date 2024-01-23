---
layout: single
title:  "Incident"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

- Incident may be caused by Changes Investigation of Incidents may indicate the need for a Change.
- You can use pre-defined constant in server-side code(Script Includes, Business Rule, UI Action)
- You can't create change request from inactive incidents.
- Inbound actions can be configured to enable creating or updating incidents.
- Category and subcategory is stored by Choice[sys_choice]
- Duration[calendar_duration] : Total elapsed time between when an incident is created until the time it's resolved.
- Reduction in the time services are unavailable.



# State

## New

![image-20240118153902504](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/25ca0a8ca8fc11de7c3b50152bc5075dcb3271e4/images/2024-01-18-servicenow_incident/image-20240118153902504.png?raw=true)

- Caller and short description are mandatory fields.
- Impact and Urgency is used to calculate priority.

## In progress



## On hold

- On hold reason is mandatory field.
- Resolved → On hold : Reopen



## Resolved

- Resolution code and Resolution notes are mandatory.
- If a user is caller and state is resolved, even if user has no roles, A user can close an incident.



## Closed

- Active : False



## Canceled

- Active : False



# Roles

- User with no assigned roles can read an incident when they are caller, opened by or on the watch list.
- VIP Users : ![image-20240118170255249](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/25ca0a8ca8fc11de7c3b50152bc5075dcb3271e4/images/2024-01-18-servicenow_incident/image-20240118170255249.png?raw=true)



# Priority Lookup Tables

![image-20240118165628716](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/25ca0a8ca8fc11de7c3b50152bc5075dcb3271e4/images/2024-01-18-servicenow_incident/image-20240118165628716.png?raw=true)



# Incident Properties



# Parent - Child Incident

- <span style='background-color: #8A2BE2'>State, Close Note, Close Code, Comments, Worknote</span> → they are updated on child incident based on parent incident update.



# Knowledge

[X] Knowledge

​	it will create a draft knowledge article once the incident is closed.



# Life Cycle

![lifecycle_incident](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-18-servicenow_incident\lifecycle_incident.jpg?raw=true)

- Creation and Classification
  - Create new & locate
  - Define & Classify
  - Assign
- Investigation and Diagnosis
  - Locate assigned incident
  - Investigate & diagnose
  - Update incident activity
  - Escalate
  - Monitor
- Resolution and Closure
  - Restore service
  - Update incident activity
  - Communicate
