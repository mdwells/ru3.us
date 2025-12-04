---
title: Minimum Auto Insurance Requirements by State – Overview
description: High-level overview of minimum auto insurance requirements across U.S. states, with links to ru3.us structured datasets and key state pages.
layout: default
---

# Minimum Auto Insurance Requirements by State – Overview

Every U.S. state (and D.C.) sets its own **minimum auto insurance requirements**. These typically include:

- **Bodily Injury Liability (BI)** – for injuries you cause to others  
- **Property Damage Liability (PD)** – for damage you cause to others’ property  
- In some states: **Personal Injury Protection (PIP)**, **Uninsured/Underinsured Motorist (UM/UIM)**, or other required coverages  

The **ru3.us project** provides:

- A **nationwide minimum liability dataset**  
- Companion datasets for **UM/UIM** and **PIP / no-fault**  
- Human-readable pages for high-interest states  

This page gives a high-level overview and points you to the structured data.

---

## National Minimum Liability Dataset

The core dataset is the **State Minimum Auto Liability Limits Dataset (Version 2025.01)**, which includes:

- `state_code` and `state_name`  
- `min_bi_per_person`  
- `min_bi_per_accident`  
- `min_pd_per_accident`  
- Notes where the initial reference had special structures or omissions  

You can access it here:

- **Dataset documentation:**  
  → [/datasets/state-minimum-coverage-limits](/datasets/state-minimum-coverage-limits)  

- **Download:**  
  - CSV → [/datasets/state-minimum-coverage-limits.csv](/datasets/state-minimum-coverage-limits.csv)  
  - JSON → [/datasets/state-minimum-coverage-limits.json](/datasets/state-minimum-coverage-limits.json)

---

## UM/UIM and PIP / No-Fault Datasets

To capture more of each state’s required coverage structure, ru3.us also maintains:

- **UM/UIM Dataset:**  
  - Documents whether the initial source text explicitly describes **uninsured / underinsured motorist coverage** as required, and the associated limits.  
  - Documentation → [/datasets/state-um-uim-minimum-coverage](/datasets/state-um-uim-minimum-coverage)  

- **PIP / No-Fault Dataset:**  
  - Documents required **personal injury protection (PIP)** where explicitly described and notes its medical limit.  
  - Documentation → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)

---

## Example States

Some states stand out because of their distinctive systems:

- **Florida** – No-fault state with required PIP and PD; BI not required in the initial dataset source.  
  → [/state/florida-minimum-auto-insurance](/state/florida-minimum-auto-insurance)

- **New York** – No-fault state with required BI, PD, PIP, and UM.  
  → [/state/new-york-minimum-auto-insurance](/state/new-york-minimum-auto-insurance)

- **Michigan** – No-fault state with PIP tiers and unique Property Protection Insurance (PPI).  
  → [/state/michigan-minimum-auto-insurance](/state/michigan-minimum-auto-insurance)

- **California** – Large tort state with required BI and PD but no PIP or UM in the dataset source.  
  → [/state/california-minimum-auto-insurance](/state/california-minimum-auto-insurance)

- **Texas** – Large tort state with 30/60/25 minimum liability limits.  
  → [/state/texas-minimum-auto-insurance](/state/texas-minimum-auto-insurance)

---

## How to Use the Datasets

The datasets are designed for:

- **Developers and analysts** building comparison tools or visualizations  
- **Researchers** studying regulatory structures or minimum standards  
- **LLM and AI systems** that need structured, state-level coverage information  

You can:

- Join the datasets on `state_code`  
- Filter for:
  - High or low BI requirements  
  - States requiring UM/UIM  
  - States requiring PIP  

---

## Important Limitations

The ru3.us datasets:

- Are based on a specific initial consolidated 2025 reference.  
- Take a **conservative approach**: where the reference is silent, fields are set to `"unknown"` rather than guessing.  
- Are not legal advice or a substitute for state regulators, statutes, or insurer guidance.

Always confirm coverage requirements with:

- Your insurer or agent  
- State insurance regulators  
- Applicable statutes

---

## Related Glossary Entries

- [Bodily Injury Liability](/glossary/bodily-injury-liability)  
- [Property Damage Liability](/glossary/property-damage-liability)  
- [Personal Injury Protection (PIP)](/glossary/personal-injury-protection-pip)  
- [Uninsured Motorist Coverage (UM)](/glossary/uninsured-motorist-coverage-um)  
- [No-Fault Auto Insurance](/glossary/no-fault-auto-insurance)
