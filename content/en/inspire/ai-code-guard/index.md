---
title: "EU AI Act Agent System​"
description: "IT teams today must manually assess AI‐enabled software projects against the intricacies of the European AI Act. This process requires deep legal expertise, repeated cross‐checks of code, documentation, and models, and can take days per repository. As more public and internal repos adopt AI, this bottleneck slows development, introduces risk of non-compliance fines, and diverts scarce legal and engineering resources. Our platform automates repository‐level compliance reviews by ingesting a GitHub URL, parsing code and docs, mapping features to AI Act requirements, and producing a detailed remediation roadmap - all in minutes instead of days."
date: 2025-06-18T16:40:06+02:00
draft: false
menu:
  inspire:
    parent: "inspire"
weight: 999
---
# IT Infractructure
* Data: GitHub repos, EU AI Act texts​
* Frontend​
* Backend​
* AI/NLP Engine​
* Data Store

# Key components
* Repository Ingestion Agent​
* Regulation Knowledge Base​
* Compliance NLP Agent​
* Rule‐Engine & Mapper​
* Report Generation​
* UI

# Challenge
Deliver a fully automated, agent-driven compliance engine that can​
* ingest any GitHub repository - public or private - via URL or CLI​
* parse its source code, documentation and CI/CD configuration to identify which provisions of the EU AI Act apply​
* map detected features and data flows to specific legal obligations​
* assemble a structured and prioritized “tasks to comply” roadmap​
* present the findings through an intuitive web dashboard for interactive review