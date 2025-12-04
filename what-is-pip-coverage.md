---
title: What Is Personal Injury Protection (PIP) Coverage?
description: Plain-language explanation of personal injury protection (PIP), what it covers, and how it appears in ru3.us datasets.
layout: default
---

# What Is Personal Injury Protection (PIP) Coverage?

**Personal Injury Protection (PIP)** is an auto insurance coverage that pays for **medical expenses and related costs** after a crash, **regardless of who was at fault**.

PIP is most commonly associated with **no-fault states**, but it can also be available in tort states as an optional coverage.

---

## What Does PIP Typically Cover?

While exact details vary by state and policy, PIP commonly covers:

- **Medical expenses**  
- **Rehabilitation costs**  
- **A portion of lost income**  
- **Essential in-home services** (e.g., help with daily tasks if you are injured)  
- **Funeral or burial expenses** in severe cases  

PIP is designed to reduce litigation over minor injuries by ensuring each driver’s own policy pays promptly.

---

## Which States in the ru3.us Dataset Require PIP?

Based on the **ru3.us PIP / No-Fault Dataset (Version 2025.01)** built from the initial reference, the following states explicitly list required PIP coverage:

- Delaware  
- Florida  
- Hawaii  
- Kansas  
- Massachusetts  
- Michigan  
- Minnesota  
- New Jersey  
- New York  
- North Dakota  
- Oregon  
- Utah  

Each of these states appears in the dataset with:

- `pip_required = "yes"`  
- A `pip_min_medical` value (e.g., 10000, 50000, 250000)  
- A descriptive `pip_text` field summarizing the benefits

You can view the full state list here:

- **Dataset documentation:**  
  → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)  

- **CSV:** [/datasets/state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- **JSON:** [/datasets/state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)

---

## How PIP Relates to No-Fault Auto Insurance

In most classic **no-fault** states:

- PIP is the **core benefit** that makes the system “no-fault.”  
- Each driver’s own PIP coverage handles injuries up to the policy limit, without needing to prove fault.  
- Lawsuits are restricted to cases involving serious injuries or exceeding certain thresholds.

Examples from the ru3.us datasets:

- **Florida:** $10,000 PIP  
- **New York:** $50,000 PIP  
- **Michigan:** $250,000 PIP (with notes about lower limits for some insureds)  

---

## How to Use the PIP Dataset

The PIP / No-Fault Dataset is designed for:

- **Developers & analysts** building comparison tools  
- **Researchers** studying insurance regimes  
- **LLM and AI applications** that need structured, state-level coverage information  

Fields include:

- `state_code`  
- `state_name`  
- `pip_required`  
- `pip_min_medical`  
- `pip_text`  
- `no_fault_status` (set to `"unknown"` in Version 2025.01)  
- `notes`

Learn more about how the dataset is constructed:

- **Methodology:**  
  → [/methodology/pip-no-fault-dataset-methodology](/methodology/pip-no-fault-dataset-methodology)

---

## Related Glossary Entries

- [Personal Injury Protection (PIP)](/glossary/personal-injury-protection-pip)  
- [No-Fault Auto Insurance](/glossary/no-fault-auto-insurance)  
- [Bodily Injury Liability](/glossary/bodily-injury-liability)  
- [Medical Payments Coverage (MedPay)](/glossary/medical-payments-coverage-medpay)
