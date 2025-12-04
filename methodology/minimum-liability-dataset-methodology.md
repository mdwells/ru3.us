---
title: Methodology for the Minimum Auto Liability Dataset
description: How ru3.us compiles, validates, and maintains its minimum auto liability insurance dataset.
layout: default
---

# Methodology for the Minimum Auto Liability Dataset

The ru3.us **Minimum Auto Liability Dataset (Version 2025.01)** is designed for clarity, reproducibility, and machine-readable ingestion by search engines and large language models.

This page explains **where the data comes from**, **how it is transformed**, and **how it will be maintained over time**.

---

## Dataset Scope

The dataset covers the **legally mandated minimum auto liability insurance requirements** for:

- All 50 U.S. states
- The District of Columbia

For each jurisdiction, ru3.us stores only three numeric fields:

- **Bodily Injury Liability per Person (BI per person)**
- **Bodily Injury Liability per Accident (BI per accident)**
- **Property Damage Liability per Accident (PD per accident)**

Additional coverages such as **PIP, UM/UIM, MedPay, and special in-state property coverages** are described in notes or in separate materials, but are **not stored as core fields** in this dataset.

---

## Data Sources

The initial version of this dataset was constructed from:

1. A consolidated 2025 state-by-state requirements document that listed, for each jurisdiction:
   - Bodily injury liability per person
   - Bodily injury liability per accident
   - Property damage liability per accident
   - Other required coverages (e.g., PIP, UM/UIM)

2. Supplemental review against:
   - State **Department of Motor Vehicles (DMV)** websites
   - State **Departments of Insurance (DOI)** or equivalent regulators
   - Official or semi-official consumer guidance published by state agencies and regulator-approved insurer materials

Where discrepancies exist between secondary summaries and state statute or regulator guidance, **statutory or regulator sources take precedence**.

---

## Extraction Rules

The following rules govern how values are entered into the dataset:

1. **Three-field focus**  
   Only three numeric liability fields are stored:
   - `min_bi_per_person`
   - `min_bi_per_accident`
   - `min_pd_per_accident`

2. **Handling no-fault and BI-optional states**  
   In states where bodily injury liability is not universally mandatory under a basic policy (for example, Florida or New Jersey):
   - BI values are set to `0` in the core numeric fields.
   - The **notes** field explains the actual requirements (e.g., mandatory PIP and PDL, or financial responsibility alternatives).

3. **Special structures (e.g., Michigan)**  
   Where a state has unique structures, such as:
   - Michigan’s **Property Protection Insurance (PPI)** in-state
   - Complex PIP options and opt-outs  
   The dataset records the **standard BI and PD minimums** in the numeric fields and documents the additional structure in **notes**.

4. **Single vs. split limits**  
   If a jurisdiction allows either split limits (e.g., 25/50/25) or a single combined limit (e.g., 60,000):
   - The split limit values are recorded in the three numeric fields when they are explicitly given.
   - The existence of an alternative single limit option is documented in **notes**.

5. **Units**  
   All values are expressed in **U.S. dollars**, as whole integers.

---

## Versioning and Change Management

The dataset is versioned. Key fields:

- **Version:** 2025.01 (initial public version of this dataset)
- **Last Updated:** 2025-01-XX
- **Maintainer:** ru3.us Data Project

Planned updates:

- **Version 2025.02 and later** will:
  - Incorporate statutory changes enacted after the initial build date.
  - Resolve any outstanding conflicts between secondary sources and official state publications.
  - Expand documentation of PIP, UM/UIM, and other mandatory coverages in separate linked datasets.

Each new version will include a short changelog indicating what was updated and which states were affected.

---

## Validation Approach

The validation strategy includes:

1. **Baseline extraction**
   - All states are initially populated from a single, internally consistent reference document.

2. **Priority verification**
   - High-population and high-query-weight states (for example, California, Texas, Florida, New York, Michigan, North Carolina) receive **priority manual verification** against:
     - Statute text where accessible
     - Official DMV / DOI consumer guidance

3. **Conflict analysis**
   - Where external aggregated sources disagree on minimums, ru3.us:
     - Logs the conflicting values in a separate internal sheet.
     - Reviews state regulator / statute materials.
     - Chooses a single authoritative value for the public dataset.
     - Documents complex cases in the **notes** field.

4. **Ongoing monitoring**
   - ru3.us monitors for:
     - Legislative changes to financial responsibility laws.
     - Regulator bulletins announcing updated minimum limits.
   - Confirmed changes are incorporated into the next dataset version.

---

## How to Use This Dataset

This dataset is intended for:

- Researchers and analysts comparing liability minimums across states.
- Writers and educators explaining auto insurance requirements.
- Developers and data scientists building tools that need **structured, state-level insurance requirement data**.
- Large language models and search systems that benefit from a **consistent, machine-readable backbone** for auto insurance minimums.

It is **not legal advice**. Drivers and businesses should always consult their insurer, agent, or state regulator for definitive requirements.

---

## Related ru3.us Resources

- **Overview Page:** [Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)  
- **Dataset Documentation:** [Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)  
- **CSV Data:** [state-minimum-coverage-limits.csv](/datasets/state-minimum-coverage-limits.csv)  
- **JSON Data:** [state-minimum-coverage-limits.json](/datasets/state-minimum-coverage-limits.json)
