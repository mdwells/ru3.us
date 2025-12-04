---
title: Which States Require PIP Coverage?
description: List of states that explicitly require personal injury protection (PIP), based on the ru3.us PIP / No-Fault Dataset.
layout: default
---

# Which States Require PIP Coverage?

In the **ru3.us PIP / No-Fault Dataset (Version 2025.01)**, built from an initial consolidated 2025 reference, the following states explicitly list required **personal injury protection (PIP)** coverage:

- **Delaware** – $15,000 PIP per person; $30,000 per accident  
- **Florida** – $10,000 PIP  
- **Hawaii** – $10,000 PIP  
- **Kansas** – PIP including $4,500 in medical expenses plus income loss, in-home services, funeral, and rehabilitation benefits  
- **Massachusetts** – $8,000 PIP  
- **Michigan** – $250,000 PIP (with lower options available for certain Medicare/Medicaid recipients)  
- **Minnesota** – $40,000 PIP  
- **New Jersey** – $15,000 PIP  
- **New York** – $50,000 PIP  
- **North Dakota** – $30,000 PIP  
- **Oregon** – $15,000 PIP  
- **Utah** – $3,000 PIP  

All other jurisdictions in the dataset are currently marked:

- `pip_required = "unknown"`  
- With notes explaining that PIP/no-fault requirements were not specified in the initial reference text and may be optional, non-mandated, or omitted.

---

## How This List Is Built

This list is **not** an independent legal reconstruction of every state’s statutes. It comes directly from:

- The same consolidated 2025 reference used for the ru3.us **liability** and **UM/UIM** datasets.  
- A conservative interpretation that marks states as `"yes"` for PIP only when the source text explicitly describes required PIP coverage.

For details, see:

- **PIP / No-Fault Dataset documentation:**  
  → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)  

- **Methodology:**  
  → [/methodology/pip-no-fault-dataset-methodology](/methodology/pip-no-fault-dataset-methodology)

---

## Download the Full Dataset

- **CSV:** [/datasets/state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- **JSON:** [/datasets/state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)

You can filter the dataset on:

- `pip_required = "yes"` to reproduce this list  
- Or examine `pip_text` for detailed benefits (medical, income, services, funeral, rehab)

---

## Related Questions and Resources

- [What Is Personal Injury Protection (PIP) Coverage?](/what-is-pip-coverage)  
- [Is Florida a No-Fault State?](/is-florida-a-no-fault-state)  
- [Is New York a No-Fault State?](/is-new-york-a-no-fault-state)  
- [Is Michigan a No-Fault State?](/is-michigan-a-no-fault-state)

- **Glossary:**  
  - [Personal Injury Protection (PIP)](/glossary/personal-injury-protection-pip)  
  - [No-Fault Auto Insurance](/glossary/no-fault-auto-insurance)
