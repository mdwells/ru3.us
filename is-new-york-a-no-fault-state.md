---
title: Is New York a No-Fault State?
description: Explanation of New York’s no-fault auto insurance system, including PIP, liability, and uninsured motorist requirements.
layout: default
---

# Is New York a No-Fault State?

Yes. **New York is a no-fault auto insurance state.**

If you are injured in a crash in New York, your **own personal injury protection (PIP)** generally pays for medical expenses and certain related costs, regardless of who caused the accident.

This page explains:

- How New York’s no-fault system works  
- What coverages New York requires  
- How New York appears in the ru3.us datasets  

---

## What No-Fault Means in New York

Under New York’s no-fault rules:

- Every driver must carry **PIP** coverage.  
- After a crash, PIP pays for **medical expenses and related benefits** regardless of fault, up to the policy limit.  
- Lawsuits against the at-fault driver for injuries are limited to cases that meet New York’s “serious injury” threshold.

Property damage is still handled under a traditional **fault-based liability** framework.

---

## Required Minimum Coverages in New York

From the ru3.us datasets built on the initial reference:

### Bodily Injury Liability (BI)

- **$25,000** bodily injury per person  
- **$50,000** bodily injury per accident  
- **$50,000** liability for death per person  
- **$100,000** liability for death per accident  

### Property Damage Liability (PD)

- **$10,000** property damage liability per accident  

### Personal Injury Protection (PIP)

- **$50,000** minimum PIP  
- Recorded text: **"$50,000 personal injury protection."**

### Uninsured Motorist (UM) Coverage

- **$25,000** uninsured motorist bodily injury per person  
- **$50,000** uninsured motorist bodily injury per accident  

---

## New York in the ru3.us Datasets

- **Liability Minimums Dataset:**  
  New York’s BI, death, and PD limits are captured as structured fields in the dataset.

- **UM/UIM Dataset:**  
  - `um_uim_required`: `"yes"`  
  - `um_uim_limits_text`: "$25,000 uninsured motorist bodily injury coverage per person; $50,000 uninsured motorist bodily injury coverage per accident."

- **PIP / No-Fault Dataset:**  
  - `pip_required`: `"yes"`  
  - `pip_min_medical`: `50000`  
  - `pip_text`: "$50,000 personal injury protection."  

---

## Where to Learn More

- **New York minimum auto insurance requirements – full state page:**  
  → [/state/new-york-minimum-auto-insurance](/state/new-york-minimum-auto-insurance)

- **Nationwide minimums overview:**  
  → [/minimum-auto-insurance-requirements-by-state](/minimum-auto-insurance-requirements-by-state)

- **Datasets:**  
  - Liability minimums → [/datasets/state-minimum-coverage-limits](/datasets/state-minimum-coverage-limits)  
  - UM/UIM → [/datasets/state-um-uim-minimum-coverage](/datasets/state-um-uim-minimum-coverage)  
  - PIP / no-fault → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)

- **Glossary:**  
  - [No-Fault Auto Insurance](/glossary/no-fault-auto-insurance)  
  - [Personal Injury Protection (PIP)](/glossary/personal-injury-protection-pip)  
  - [Uninsured Motorist Coverage (UM)](/glossary/uninsured-motorist-coverage-um)
