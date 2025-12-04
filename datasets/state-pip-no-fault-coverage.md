---
title: State Personal Injury Protection (PIP) and No-Fault-Related Coverage – Dataset
description: Dataset documenting personal injury protection (PIP) amounts where specified, and placeholders for no-fault classification, based on an initial 2025 state requirements reference.
layout: default
---

# State Personal Injury Protection (PIP) and No-Fault-Related Coverage – Dataset

The **ru3.us PIP / No-Fault Dataset (Version 2025.01)** captures where an initial consolidated 2025 reference explicitly describes **personal injury protection (PIP)** requirements and associated minimum amounts.

This dataset is intentionally conservative: it **only** marks PIP as required where the source text clearly states it, and leaves both PIP and no-fault classification as `"unknown"` elsewhere rather than guessing.

---

## Dataset Scope

For each jurisdiction (50 states + D.C.), the dataset records:

- `state_code` – two-letter USPS abbreviation  
- `state_name` – full state name  
- `pip_required` – `"yes"` where the source text explicitly describes PIP as part of the required coverage; `"unknown"` otherwise  
- `pip_min_medical` – numeric PIP medical coverage amount when clearly described (e.g., 10000 for $10,000), blank otherwise  
- `pip_text` – full PIP description as given in the source text (e.g., PIP medical, income loss, and related benefits)  
- `no_fault_status` – `"unknown"` in Version 2025.01 for all jurisdictions (future versions may classify tort vs. no-fault vs. choice based on statutory review)  
- `notes` – primarily used to explain missing or unspecified PIP/no-fault requirements

---

## Access the Dataset

- **CSV:** [state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- **JSON:** [state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)  

For methodology and design decisions, see:

- **[Methodology for the PIP / No-Fault Dataset](/methodology/pip-no-fault-dataset-methodology)**

---

## Relationship to Other ru3.us Datasets

This dataset is designed to complement:

- **[State Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)**  
- **[State UM/UIM Coverage Dataset](/datasets/state-um-uim-minimum-coverage)**  

Together, the three datasets provide:

- Liability minimums  
- UM/UIM requirements (where specified)  
- PIP and PIP-like benefits (where specified)

Future versions may integrate a verified **no-fault classification** and deeper PIP/benefit breakdown.

---

## Version Information

- **Dataset:** State PIP / No-Fault Coverage  
- **Version:** 2025.01  
- **Last Updated:** 2025-01-XX  
- **Maintainer:** ru3.us Data Project  

---

## Related ru3.us Resources

- [Datasets Index](/datasets/)
- [Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)
- [State Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)
- [State UM/UIM Coverage Dataset](/datasets/state-um-uim-minimum-coverage)
- [Methodology for the PIP / No-Fault Dataset](/methodology/pip-no-fault-dataset-methodology)
- [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)
- [Methodology for the UM/UIM Dataset](/methodology/um-uim-dataset-methodology)
