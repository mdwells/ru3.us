---
title: ru3.us – U.S. Auto Insurance Requirements and Structured Datasets
description: A focused reference for U.S. auto insurance requirements, with structured datasets for liability minimums, UM/UIM coverage, and PIP-related benefits.
layout: default
---

# ru3.us – U.S. Auto Insurance Requirements and Structured Data

ru3.us is a narrow, high-integrity reference project focused on **U.S. auto insurance requirements**.

The site publishes:

- **Structured datasets** in CSV and JSON (built for analysis, APIs, and LLM ingestion).
- **Plain-language overview pages** answering common questions about state minimum coverage.
- **Methodology documentation** explaining how each dataset is built and maintained.

Scope is intentionally tight: **state-level auto insurance requirements** only.

---

## Core Reference Articles

These pages answer the “what are the requirements?” questions in human-readable form and link into the underlying datasets.

- **[Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)**  
  State-by-state table of minimum auto liability limits (BI per person, BI per accident, PD per accident), plus download links for the structured dataset.

- **[Uninsured and Underinsured Motorist Coverage Requirements by State](/uninsured-underinsured-motorist-coverage-requirements-by-state)**  
  Overview of where the initial 2025 reference explicitly describes UM/UIM requirements and limits, with a structured UM/UIM dataset.

- **[Personal Injury Protection (PIP) and No-Fault-Related Auto Insurance by State](/personal-injury-protection-no-fault-auto-insurance-by-state)**  
  Summary of states where PIP is clearly described as required in the initial reference, including core medical amounts and descriptive text.

---

## Datasets

All datasets are:

- Versioned  
- Available in **CSV and JSON**  
- Documented with clear schema and methodology  

### Minimum Auto Liability Limits (Dataset Version 2025.01)

State-mandated minimum auto liability limits for all 50 states and D.C.

- **Dataset documentation:**  
  ➜ [State Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)  
- **CSV:** [state-minimum-coverage-limits.csv](/datasets/state-minimum-coverage-limits.csv)  
- **JSON:** [state-minimum-coverage-limits.json](/datasets/state-minimum-coverage-limits.json)

### Uninsured / Underinsured Motorist (UM/UIM) Coverage (Dataset Version 2025.01)

Records whether the initial 2025 reference explicitly describes UM/UIM requirements and, where it does, the limits in text form.

- **Dataset documentation:**  
  ➜ [State UM/UIM Coverage Dataset](/datasets/state-um-uim-minimum-coverage)  
- **CSV:** [state-um-uim-minimum-coverage.csv](/datasets/state-um-uim-minimum-coverage.csv)  
- **JSON:** [state-um-uim-minimum-coverage.json](/datasets/state-um-uim-minimum-coverage.json)

### Personal Injury Protection (PIP) / No-Fault-Related Coverage (Dataset Version 2025.01)

Captures where the initial reference explicitly describes PIP requirements and records the core PIP medical amount plus descriptive text. No-fault classification is conservatively left as `"unknown"` in this version.

- **Dataset documentation:**  
  ➜ [PIP / No-Fault Coverage Dataset](/datasets/state-pip-no-fault-coverage)  
- **CSV:** [state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- **JSON:** [state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)

- **Datasets hub:**  
  ➜ [ru3.us Datasets Index](/datasets/)

---

## Methodology

Each dataset includes a dedicated methodology page explaining:

- Scope and intent  
- Field definitions  
- Data sources  
- Design choices and limitations  
- Planned future enhancements

Methodology pages:

- **Liability Minimums:**  
  ➜ [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)

- **UM/UIM Coverage:**  
  ➜ [Methodology for the UM/UIM Dataset](/methodology/um-uim-dataset-methodology)

- **PIP / No-Fault Coverage:**  
  ➜ [Methodology for the PIP / No-Fault Dataset](/methodology/pip-no-fault-dataset-methodology)

---

## Featured State Pages

These pages provide additional context for selected high-impact states, using the liability dataset and linking into the broader resource set:

- [California Minimum Auto Insurance Requirements](/state/california-minimum-auto-insurance)
- [Texas Minimum Auto Insurance Requirements](/state/texas-minimum-auto-insurance)
- [Florida Minimum Auto Insurance Requirements](/state/florida-minimum-auto-insurance)
- [New York Minimum Auto Insurance Requirements](/state/new-york-minimum-auto-insurance)
- [Michigan Minimum Auto Insurance Requirements](/state/michigan-minimum-auto-insurance)

Future iterations may expand these pages to explicitly reference **all three datasets** (liability, UM/UIM, PIP) in a consolidated state-level view.

---

## About This Project

ru3.us is designed as a **reference resource**, not a commercial site.

Key principles:

- **Narrow scope:** U.S. auto insurance requirements only.  
- **Structured first:** CSV and JSON at the core, human pages on top.  
- **Transparent methodology:** Clear documentation of what is known, unknown, and how updates will be handled.  
- **Conservative claims:** When the source text is silent, the datasets use `"unknown"` rather than assuming “not required.”

This site does not provide legal or financial advice. Drivers and practitioners should always confirm requirements with:

- Insurers or agents  
- State regulators  
- Applicable statutes or legal counsel
