---
layout: single
title:  "Problem"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

# Knowledge
## Articles
### Unknown Error Articles
- plugin : com.snc.best_practice.problem.madrid.knowledge

![image-20240116161800231](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/611c332dcb52e6037b4f0adf9b8e9d5fb4315677/images/2024-01-16-servicenow1/image-20240116161800231.png?raw=true)

### Access
- User Criteria and User Roles

# State
### New

![image-20240118163211192](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163211192.png?raw=true)

- Mandatory field : Problem statement
- When you insert problem statement, Related Search is auto-populated.
- Button : Assess



### Assess

- Mandatory field : Assign to

![image-20240118163424077](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163424077.png?raw=true)

 → Mandatory field dialog pop-up.

![image-20240118163534732](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163534732.png?raw=true)

- Button

  - Confirm

    → Root Cause Analysis

  - Mark Duplicate

    ![image-20240118163709350](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163709350.png?raw=true)

  - Cancel

    ![image-20240118163737705](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163737705.png?raw=true)



### Root Cause Analysis

- Button

  - Fix

    ![image-20240118164132131](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118164132131.png?raw=true)

  - Mark Duplicate

  - Cancel

  - Accept Risk

    ![image-20240118163959170](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118163959170.png?raw=true)

    *state can be changed on problem property.*



### Fix in Progress

- Button
  - Resolve
  - Re-Analyze : Go back to Root Cause Analysis.
  - Accept Risk



### Resolved

- Button
  - Complete
  - Re-Analyze



### Closed



### Problem Task

- moving a problem task from one state to another : ProblemTaskStateUtils

# Roles
## ![IMG_3498](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/611c332dcb52e6037b4f0adf9b8e9d5fb4315677/images/2024-01-16-servicenow1/IMG_3498.jpg?raw=true)

- Admin and problem_admin have all of roles except for updating related incidents count

## Problem_Task_Analyst

- Can Create problem task
- Can Read
- Can Update problem task
- Can Close problem task
- Cannot Delete problem task!!!

## Problem_Coordinator

- Have all of roles what problem_admin have, but <span style='background-color: #8A2BE2'>Cannot Delete & Manage problem properties</span>!!

## ITIL

- Have all of roles what itil_admin have, but <span style='background-color: #8A2BE2'>Cannot Delete</span>!!

## ITIL_Admin

- Can Create
- Can Read
- Can Update
- Can Delete
- Add related Incidents
- <span style='background-color: #8A2BE2'>Cannot Close</span>
- <span style='background-color: #8A2BE2'>Cannot Communicate workaround, fix</span>
- <span style='background-color: #8A2BE2'>Cannot Create known error articles</span>
- <span style='background-color: #8A2BE2'>Cannot Manage problem properties</span>



# Virtual Agent

## How to use virtual agent

1. Go to Service Portal Configuration
2. Go to Designer
3. Search "index"
4. Go to home page index
5. Search "virtual agent"
6. Use virtuall agent service portal widget

![image-20240116162338677](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/611c332dcb52e6037b4f0adf9b8e9d5fb4315677/images/2024-01-16-servicenow1/image-20240116162338677.png?raw=true)



## Available Topic Blocks

- Search Catalog Item
- Request Catalog
- Create Incident



# Problem Properties

[ ] Accept Risk moves the Problem to Closed state instead of Resolved state

[ ] Can create a Problem Task on a Closed Problem?

[ ] Cancel open Problem Tasks when closing a Problem

[ ] Can Re-Assess a Problem Task on a Closed Problem?

[ ] Copy attachments from the incident

[ ] Allow problem creation from interaction

[ ] Create saved problem (interaction)

- Who can Re-analyze a Canceled Problem? ( & admin)

- Who can Re-analyze a Risk Accepted (Closed state) Problem?
- Who can Re-analyze a Completed Problem?
- Who can relate closed Incidents to a Problem?
- Who can Re-assess a Completed or Canceled Problem Task?

![image-20240118164933209](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118164933209.png?raw=true)

![image-20240118164947399](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/81f188fe28c5ef0fa91f97e9e36cc6416f562ded/images/2024-01-16-servicenow1/image-20240118164947399.png?raw=true)

  
