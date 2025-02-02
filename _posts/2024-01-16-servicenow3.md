---
layout: single
title:  "Knowledge"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

# Version

- PlugIn : Knowledge Management Advanced Installer

## Legacy

- Categorization

## V2

- Topic and Category and taxonomy shared by all articles.

## V3

- multi level of categorizations
- each kb has its own taxonomy



# Tables

![image-20240116164150333](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/4b2f37ea9aea4b1b5ba064ed431cd8f95bfc0a92/images/2024-01-16-servicenow3/image-20240116164150333.png?raw=true)

- ts_query_kb

### FeedBack [kb_feedback]

- Flags
- Helpful(Yes/No)
- Comments
- Star Rating



# Roles

- Can Contribute
- Cannot Contribute
- Can Read
- Cannot Read
- <span style='background-color: #8A2BE2'>using user criteria</span>



# Modules

![image-20240118153140673](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/7d745b350e35dac48b852330ca2d3c3af4ed221d/images/2024-01-16-servicenow3/image-20240118153140673.png?raw=true)

- Search keyword : Knowledge > Administration > Search Log



# Workflow

- Knowledge - Instant Publish
- Knowledge - Approval Publish
- Knowledge -  Instant Retire
- Knowledge - Approval Retire



# Knowledge base

- KB can have own workflow.

- Base table for Knowledge [kb_knowledge]



# Articles

- featured content (kb_knowledge_keyword)

![image-20240118152456904](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/7d745b350e35dac48b852330ca2d3c3af4ed221d/images/2024-01-16-servicenow3/image-20240118152456904.png?raw=true)

- It's stored in kb_knowledge.

## State

- Draft → Review → Scheduled for publish → Published

- Pending retirement → Retired
- Outdated

## Creating way

- Direct creation by a user with the 'knowledge' role.
- Import from a Microsoft Word document.
- Generated from Incident or problem records.
