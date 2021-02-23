---
title: XtrfProject
description: 'Creates a project in XTRF automatically'
position: 2
version: 1.0
category: 'workflows'
---

## Description

Creates a project in XTRF automatically

## Steps

1. Search files on a defined destination
2. Grabs the files
3. If OCR is True, sends the files for OCR
4. If batch is True, creates a project in XTRF with all the files including OCR
5. Start tasks if set
6. Sends a notification of the created project

## Parameters

### Workflow Paramaters

| Parameter         | Description                                               | Options    |
| ----------------- | --------------------------------------------------------- | ---------- |
| batch             | when false, it processes each file as a separated project | True/False |
| start_tasks       | when true, it will automatically start the tasks          | True/False |
| ocr_active        | process files to OCR and adds output to the project       | True/False |
| ocr_languages     | language of the documents for the OCR                     | english    |
| ocr_output_format | output format from the OCR                                | txt        |
| download_prefix   | folder where the files are storaged                       | required   |
| type              | either project or quote                                   | required   |

### Project Paramaters

| Parameter          | Description               | Options                |
| ------------------ | ------------------------- | ---------------------- |
| customer           | ---                       | required               |
| person_responsible | project manager assigned  | required               |
| source_language    | ---                       | required               |
| target_languages   | ---                       | multiple               |
| service            | ---                       | required               |
| specialization     | ---                       | required               |
| categories         | ---                       | multiple               |
| custom_fields      | ---                       | multiple               |
| service            | ---                       | required               |
| deadline           | expressed in working days | required               |
| name_option        | predefined dynamic name   | DATE: adds current day |
| name_prefix        | predefined static name    | Text                   |

### Administrative Parameters (systems only)

| Parameter         | Description | Options  |
| ----------------- | ----------- | -------- |
| download_prefix   | ---         | required |
| download_link_url | ---         | required |
| template          | ---         | required |
