---
layout: single
title:  "Change"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

![image-20240116164530078](../images/2024-01-16-servicenow4/image-20240116164530078.png?raw=true)

- Change Type : <span style='background-color: #fff5b1'>Emergency, Normal, Standard(Preapproved)</span>



# Normal Change

![image-20240116164651971](../images/2024-01-16-servicenow4/image-20240116164651971.png?raw=true)

## State

New → Assess → Authorize → Scheduled → Implement → Review → Closed / Canceled

### New

When you submit change without any information,

​	Automate populated : Requested by, Category(Other), Priority(4 - Low), Risk(Morderate), Impact(3 - Low)

To request approval, Assignment group field have to be populated.



### Assess

No one approved.



### Authorize

Anyone has approved, but not all approvers have approved.



### Scheduled



### Implement



### Review



### Closed

- Mandatory field : Close code, Close notes



# Standard Change

- it doesn't require approvals.

## Standard change template

- it requires approvals.
- How to use template

![image-20240116171418251](../images/2024-01-16-servicenow4/image-20240116171418251.png?raw=true)

- Create New template

![image-20240116171459566](../images/2024-01-16-servicenow4/image-20240116171459566.png?raw=true)

![image-20240116171611930](../images/2024-01-16-servicenow4/image-20240116171611930.png?raw=true)

## State

New → Scheduled → Implement → Review → Close / Canceled

### Scheduled 

- Assignment group is mandatory field.

### Close

- Mandatory field : Close code, Close notes



# Task



# Incident

- You can create only one change request from an incident.

![image-20240116173710656](../images/2024-01-16-servicenow4/image-20240116173710656.png?raw=true)

**After creating change, there is no option for change.**

![image-20240116173809331](../images/2024-01-16-servicenow4/image-20240116173809331.png?raw=true)



# Roles

![changerole](../images/2024-01-16-servicenow4/changerole.jpg?raw=true)
