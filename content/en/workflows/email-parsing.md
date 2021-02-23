---
title: EmailParsing
description: 'Parses the necessary fields to create a XTRF Project from an email based on a defined template'
position: 3
version: 1.0
category: 'workflows'
---

## Description

Parses the necessary fields to create a XTRF Project from an email based on a defined template

## Setup

1. Have an email example to create the template
2. Identify which fields will be parsed from the email
3. Set fixed fields
4. Set from which will come from and to who will be directed
5. Create necessary rules to identify the email and match it with the template

## Steps

1. Make sure to have the setup correctly
2. Receive email to an specific address
3. Parse fields from the email
4. Grab the attachment
5. Dispatch XtrfProject workflow [(see more)](/workflows/xtrf-project)

## Parameters

### Workflow Paramaters

Same as the XtrfProject workflow [(see more)](/workflows/xtrf-project)

### Administrative Parameters (systems only)

| Parameter | Description                                                                                                                                                                                                | Options |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| mapping   | - default_prefix<br>- entities<br> - field<br> - type: string\|number\|array\|date<br> - label<br> - label_inside<br> - entity<br> - field<br> - suffix<br> - prefix<br> - format (date only)<br> <br><br> |         |
