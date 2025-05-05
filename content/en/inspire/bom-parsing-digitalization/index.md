---
title: "PCBA BOM Parsing & Digitalization"
description: "In the electronics industry, there is no standardized format for Bills of Materials (BOMs) for Printed Circuit Board Assemblies (PCBAs). Customers typically provide BOMs in various structures and file types (e.g., Excel, CSV, PDF), often tailored to their internal processes. This diversity makes automated processing and digitalization of BOMs challenging."
date: 2023-08-23T16:40:06+02:00
draft: false
menu:
  inspire:
    parent: "inspire"
    identifier: "industry-104569020912ec29a20eef119f0db4ec"
weight: 999
---
# IT Infractructure
* BOM files in various formats/layouts/structures
* UI / Application hosting environment
* LLMs

# Key components
* Parsing Engine: Automatic extraction and interpretation of BOM content using AI/NLP techniques
* Uncertainty Detection
* Human interaction for feedback loop

# Challenge
Develop a working prototype that accepts BOMs in different formats and transforms them into a unified, structured format.

The system must be able to identify uncertainty in its parsing results and explicitly highlight areas where manual human validation is needed.

The ultimate goal is to achieve high parsing accuracy and ensure traceability of decisions, incorporating a human-in-the-loop where necessary.