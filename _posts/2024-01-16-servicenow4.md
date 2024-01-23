---
layout: single
title:  "Change"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

![image-20240116164530078](../images/2024-01-16-servicenow4/image-20240116164530078.png?raw=true)

- Change Type : <span style='background-color: #8A2BE2'>Emergency, Normal, Standard(Preapproved)</span>

- Life Cycle : Creation and scope → Approval → Implementation → Closure

- Conflict detection : Change > Administration > Conflict Properties
  - CI / 부모 CI / 자식 CI 에게 같은 시간에 이미 스케쥴이 잡혀 있을 때
  - CI / 부모 CI / 자식 CI 가 maintenance window에 있지 않을 때
  - CI / 부모 CI / 자식 CI 가 blackout window에 있을 때
  - assigned person에게 같은 시간에 이미 스케쥴이 있을 때
- CAB Date is auto-populated when change is added to a CAB meeting agenda.



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



### Modify change state model

- Script Includes : ChangeRequestStateModel
- Table : Model States (sttrm_state)



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

## Task workflow

- It includes standard, administrative tasks common to all Normal changes

# Incident

- You can create only one change request from an incident.

![image-20240116173710656](../images/2024-01-16-servicenow4/image-20240116173710656.png?raw=true)

**After creating change, there is no option for change.**

![image-20240116173809331](../images/2024-01-16-servicenow4/image-20240116173809331.png?raw=true)



# Problems

- When you copy from problem into a change, attributes can be modified from UI acion script. !!!NOT PROPERTIES!!!



# Roles

![changerole](../images/2024-01-16-servicenow4/changerole.jpg?raw=true)

- Admin has all of roles.

## itil_admin + itil

- Cannot create, update and delete(but not itil) CAB definition
- Cannot facilitate and refresh CAB meeting
- Cannot create standard change proposal & policy & decision record & model

## Change_manager

- Can read change record
- Can create standard change proposal & policy & decision record & model



# Workflow

![image-20240119162708378](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-16-servicenow4\image-20240119162708378.png?raw=true)

- task : subworkflow
- approval : workflow



# Tables

### change_task_sla

- task_sla
- change_task
