---
title: Personal Injury Protection (PIP) and No-Fault-Related Auto Insurance by State
description: Overview of personal injury protection (PIP) requirements and related no-fault structures based on the ru3.us PIP / No-Fault Dataset (Version 2025.01).
layout: default
---

# Personal Injury Protection (PIP) and No-Fault-Related Auto Insurance by State

Personal injury protection (**PIP**) is a type of auto insurance coverage that helps pay for medical expenses and, in many states, related costs such as income loss, in-home services, rehabilitation, and funeral expenses—often regardless of who was at fault.

Some states clearly require PIP, and some also operate under **no-fault or modified no-fault systems**. Others treat PIP as optional or structure it differently. The **ru3.us PIP / No-Fault Dataset (Version 2025.01)** captures only what is explicitly described in an initial 2025 reference document and marks everything else as `"unknown"`.

---

## States with Explicit PIP Requirements in the Initial Source

From the initial text, the following states explicitly list PIP requirements:

- **Delaware** – $15,000 PIP per person; $30,000 per accident.  
- **Florida** – $10,000 PIP.  
- **Hawaii** – $10,000 PIP.  
- **Kansas** – PIP including $4,500 in medical expenses, $900/month for up to a year for disability or loss of income, $25/day for in-home services, $2,000 for funeral/burial/cremation, and $4,500 for rehabilitation, plus survivors’ benefits with income and in-home services components.  
- **Massachusetts** – $8,000 PIP.  
- **Michigan** – $250,000 PIP (with lower options for some Medicare/Medicaid recipients).  
- **Minnesota** – $40,000 PIP.  
- **New Jersey** – $15,000 PIP.  
- **New York** – $50,000 PIP.  
- **North Dakota** – $30,000 PIP.  
- **Oregon** – $15,000 PIP.  
- **Utah** – $3,000 PIP.

All other jurisdictions in this dataset are currently marked with:

- `pip_required = "unknown"`  
- Notes indicating that PIP / no-fault requirements were **not specified** in the initial source text.

This is intentional: the dataset is designed to be **honest about gaps**, not exhaustive.

---

## Download the PIP / No-Fault Dataset

- **CSV:** [state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- **JSON:** [state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)  

Methodology and design choices:

- **[Methodology for the PIP / No-Fault Dataset](/methodology/pip-no-fault-dataset-methodology)**

---

## How This Fits With Other ru3.us Datasets

For a more complete view of auto insurance requirements, use this dataset together with:

- **[Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)**  
- **[State Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)**  
- **[State UM/UIM Coverage Dataset](/datasets/state-um-uim-minimum-coverage)**  

Together, they give:

- Liability minimums  
- UM/UIM requirements (where specified)  
- PIP requirements and related benefits (where specified)

Future dataset versions will layer in a **verified no-fault classification** and more granular PIP benefit fields.

---

## Important Disclaimer

This page and the associated dataset summarize information extracted from a single initial reference and are **not** a full restatement of each state’s law.

- PIP and no-fault rules are often nuanced and change over time.  
- Some states may require insurers to **offer** PIP or allow waivers; that detail is not captured here unless explicitly described in the source text.

Always verify coverage requirements and options with:

- Your insurer or agent  
- State insurance regulators  
- Applicable statutes or legal counsel
