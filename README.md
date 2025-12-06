# Databricks PII Governance Framework
Automated framework for **identifying, classifying, anonymizing, and governing PII** in the Databricks Lakehouse using **Microsoft Presidio**, **PySpark**, and **Unity Catalog**.

This repository contains the full implementation of the PII Detection & Governance framework referenced in my Medium article.

## 🔍 Overview

Modern data platforms must properly protect sensitive information such as **emails**, **SSNs**, **credit card numbers**, and **free-text PII**.  
This project provides an **end-to-end framework** for:

### ✔ Identifying Sensitive Data  
Automatically scan all tables using Microsoft Presidio to detect PII in structured and unstructured fields.

### ✔ Classifying & Tagging Data  
Apply Unity Catalog tags (e.g., `PII`, `EMAIL_ADDRESS`, `IP_ADDRESS`) directly to tables and columns.

### ✔ Anonymizing PII at Scale  
Use Presidio’s anonymizers to mask, replace, or partially obfuscate PII based on entity type.

### ✔ Generating Secure, Analyst-Ready Tables  
Automatically create `_anonymized` versions of PII tables for safe downstream analytics.

### ✔ Reporting & Governance  
Track scan results, anonymization outcomes, and maintain a sensitive-data inventory.

