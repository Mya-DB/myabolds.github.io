---
layout: page
title: Fine tuning and agentic pipelines
description: Agentic automation and a fine-tuned vision-language model for diagnosing print-quality errors, built during two internships at Xerox-Lexmark.
category: work
importance: 3
related_publications: false
---

Across two internships at Xerox-Lexmark, I worked on the data and modeling layers behind print-quality diagnosis.

As a **Data Engineer Intern**, I helped build a pipeline to cleanse raw data into a customer-preferred format using Databricks' Medallion architecture, Python, and SQL, including migrating data from the Big Decisions platform into Databricks.

As a **Data Scientist Intern**, I returned to extend that pipeline with agentic automation: a Databricks prototype (PySpark, SQL, Python, LangChain) that streamlined data cleaning across the Medallion architecture, and a fine-tuned version of Microsoft's Florence vision-language model on Azure ML to classify and diagnose print-quality errors. I tracked experiments with MLflow and tuned hyperparameters with Optuna, and separately researched agentic automation using Claude and MCP servers to design prompt-driven pipelines for data cleaning and ingestion.
