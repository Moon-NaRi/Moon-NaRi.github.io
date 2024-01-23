---
layout: single
title:  "Catalog Item"
categories: servicenow
tag: [servicenow, ITSM, CIS]
toc: true
author_profile: false
---

- Service Catalog can create : Enhancement, Incident, Requested Item

# Order Guide (sc_cat_item_guide)

### Path

- Service Catalog > Catalog Definitions > Order Guides

### Cascade Variables

- If checked, it auto-populates catalog item variables with names similar to order guide variables.
- REQ contains several RITMs.

### Rule Base

- Add catalog Item

### Hide 'Add to Cart'

- T / F

### Request method

- Order / Request / Submit 



# Content Item

- Links (Article / Module)
- Template

![image-20240119171156942](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-18-servicenow_catalogItem\image-20240119171156942.png?raw=true)

- Type : KB Article, Catalog Content, Module, External Content.
- Target : New Window/Tab, Within Catalog



# Service Catalog

- OOTB demo data catalog
  - Service Catalog
  - Technnical Catalog
- Request > Requested Item(RITM) > Req



# Catalog Task

## State

- Approval : Not Yet Requested / Requested / Approved / Rejected
- State : Pending / Open / Work in Progress / Closed Complete / Closed Incomplete / Closed Skipped



# User Criteria

- Available For / Not Available For

![image-20240118161036238](https://github.com/Moon-NaRi/Moon-Nari.github.io/blob/5260e00ea482f37b5abc73be17169de8101a19b8/images/2024-01-18-servicenow_catalogItem/image-20240118161036238.png?raw=true)

- Users / Groups / Roles / Companies / Locations / Departments



# Service Request

## Requests

- State : Pending Approval / Approved / Closed Complete / Closed Incomplete / Closed Cancelled / Closed Rejected / Closed Skipped

- Life Cyle :

![request_lifecyfle](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-18-servicenow_catalogItem\request_lifecyfle.jpg?raw=true)



## Roles

![srrole](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-18-servicenow_catalogItem\srrole.jpg?raw=true)

### Itil_admin

- Only can delete catalog task

### Catalog_admin

- Only cannot delete catalog task

### Catalog_editor

- Maintain categories, catalog definitions
- Maintain, create catalog item

### Catalog_manager

- Catalog_editor + Update catalog manager



![srroleful](C:\Users\User\Documents\Workspace\Moon-Nari.github.io\images\2024-01-18-servicenow_catalogItem\srroleful.jpg?raw=true)

## Itil_admin

- Cannot update & approve request

## Itil

- Cannot update & approve request
- Cannot delete requested Item
- Cannot read catalog definition

## Catalog_manager & Catalog_editor

- Read catalog definition, catalog item, categories

## Catalog_admin

- Catalog manager + Update request



## Catalog Item

### Variable Set



#### Multi Variable Set

- :x: : Custom with Label, Label, Container―, Break, Attachment, HTML, UI Page



#### reference

- sys_popup view.



# Submitted way

- Service catalog
- Service portal
- Incident record
- Service



# Mobile

- Not supported variables : URL, HTML, Label, UI Page, IP Address, Container start
