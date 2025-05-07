---
title: "Purchase order processing"
description: "Bosch divisions buy parts and equipment from vast variety of clients. Especially for niche suppliers, written communication and contracts are paper based and not standardised. Yet, they still need to be properly processed to comply with business and legal regulations. As demand grows, manual filing requires a lot of effort and gets expensive. A flexible application that combines existing paper scanning and document archiving, optical character recognition (OCR) and automating SAP flow is supposed to minimise human effort and resulting costs."
date: 2023-08-23T16:40:06+02:00
draft: false
menu:
  inspire:
    parent: "inspire"
    identifier: "industry-104569020912ec29a20eef119f0db4ec"
weight: 999
---
# IT Infractructure
* Sample Purchase Orders
* UI / Application hosting environment
* LLMs
* DB (SQLlite as fallback)

# Key components
* Data Ingestion Agent
* Semantic Analysis Agent
* Validation and Quality Assurance Agent
* User Interface

# Challenge
Create a processing pipeline for purchase orders with unknown layout. Extract business relevant information, such as sender, recipient, ids, items, prices etc. and file them into a predefined schema. A subsequent schema validation and forwarding to an API (to DB) concludes the processing.