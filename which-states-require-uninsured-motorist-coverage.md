---
title: Which States Require Uninsured Motorist Coverage?
description: List of states that explicitly require uninsured or uninsured/underinsured motorist (UM/UIM) coverage, based on the ru3.us UM/UIM Dataset.
layout: default
---

# Which States Require Uninsured Motorist Coverage?

Based on the **ru3.us UM/UIM Dataset (Version 2025.01)**, built from an initial consolidated 2025 reference, the following jurisdictions explicitly list required **uninsured or uninsured/underinsured motorist (UM/UIM)** coverage:

- **Connecticut**  
- **Illinois**  
- **Kansas**  
- **Maine**  
- **Maryland**  
- **Massachusetts**  
- **Minnesota**  
- **Missouri**  
- **Nebraska**  
- **New Hampshire**  
- **New York**  
- **North Carolina**  
- **North Dakota**  
- **Oregon**  
- **South Carolina**  
- **South Dakota**  
- **Vermont**  
- **Virginia**  
- **West Virginia**  
- **Wisconsin**  
- **District of Columbia**

Each of these entries in the dataset includes:

- `um_uim_required = "yes"`  
- A descriptive `um_uim_limits_text` field, such as:  
  - "$25,000 uninsured motorist coverage per person; $50,000 per accident."  
  - Or combined UM/UIM bodily injury and property damage requirements.

All other jurisdictions are currently marked:

- `um_uim_required = "unknown"`  
- With notes explaining that UM/UIM requirements were not described in the initial source text and may be optional, not mandated, or omitted.

---

## How This List Was Constructed

This list is **directly derived** from the initial 2025 reference used for:

- The **minimum liability** dataset  
- The **PIP / no-fault** dataset  

The ru3.us project takes a **conservative approach**:

- UM/UIM is marked `"yes"` only when the source text explicitly describes UM or UM/UIM minimums as part of required coverage.
- Otherwise, UM/UIM is left as `"unknown"` in Version 2025.01, rather than assuming it is not required.

For exact amounts and text, see:

- **UM/UIM Dataset Documentation:**  
  → [/datasets/state-um-uim-minimum-coverage](/datasets/state-um-uim-minimum-coverage)  

- **Methodology:**  
  → [/methodology/um-uim-dataset-methodology](/methodology/um-uim-dataset-methodology)

---

## Download the Full Dataset

- **CSV:** [/datasets/state-um-uim-minimum-coverage.csv](/datasets/state-um-uim-minimum-coverage.csv)  
- **JSON:** [/datasets/state-um-uim-minimum-coverage.json](/datasets/state-um-uim-minimum-coverage.json)

You can filter on:

- `um_uim_required = "yes"` to reproduce this list  
- Examine `um_uim_limits_text` for the exact minimums, including property damage UM/UIM where applicable.

---

## Related Questions and Resources

- [What Is Uninsured Motorist Coverage (UM)?](/glossary/uninsured-motorist-coverage-um)  
- [What Is Underinsured Motorist Coverage (UIM)?](/glossary/underinsured-motorist-coverage-uim)  
- [Minimum Auto Insurance Requirements by State](/minimum-auto-insurance-requirements-by-state)

- **Datasets:**  
  - Liability minimums → [/datasets/state-minimum-coverage-limits](/datasets/state-minimum-coverage-limits)  
  - PIP / no-fault → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)
