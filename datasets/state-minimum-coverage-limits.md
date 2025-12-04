---
title: Minimum Auto Insurance Liability Requirements by State
dataset_id: state-minimum-coverage-limits
version: 2025.01
last_updated: 2025-01-01
description: >
  Minimum required auto insurance liability limits (BI/BI/PD) for all U.S. states and D.C.
  Includes bodily injury per person, bodily injury per accident, and property damage minimums.
---


# State Minimum Auto Liability Coverage Limits

## Dataset Version
**Version:** 2025.01  
**Last Updated:** 2025-01-XX  
**Maintainer:** ru3.us Data Project  

This dataset contains the legally mandated minimum auto liability coverage limits for all U.S. states and the District of Columbia. Values represent the minimum required **bodily injury liability per person**, **bodily injury liability per accident**, and **property damage liability per accident**.

---

## Source Information
The values in this dataset were **manually extracted from a consolidated state-by-state requirements document** provided during project setup.  
Where possible, individual entries were cross-checked against state insurance department, DMV, or legislative sources.  
Additional validation steps are ongoing and will be reflected in future dataset versions.

---

## Methodology
To construct this dataset:

1. The source text was parsed to identify each state's statutory minimum liability requirements.
2. Only three fields were extracted:
   - **Bodily Injury Liability per Person (BI/person)**
   - **Bodily Injury Liability per Accident (BI/accident)**
   - **Property Damage Liability per Accident (PD/accident)**
3. Other mandatory coverages (PIP, UM/UIM, MedPay, special provisions) were **not included** in the structured dataset to preserve clarity and consistency.
4. For no-fault or BI-optional states (e.g., Florida, New Jersey, New Hampshire), BI values are recorded as `0` where no statutory minimum exists, and explanatory notes are added.
5. The dataset is kept in **CSV** and **JSON** formats for machine readability and LLM ingestion.  
6. Any jurisdiction that recently revised minimums (e.g., California, North Carolina) is reflected with its updated limits.

A detailed cross-state verification audit (comparing state statutes, DOI/DMV publications, and insurer regulatory filings) is planned for Dataset Version 2025.02.

**Minimum required auto liability coverage limits by U.S. state.**

This dataset is provided as:

- CSV: `/datasets/state-minimum-coverage-limits.csv`  
- JSON: `/datasets/state-minimum-coverage-limits.json`  

## Fields

- **state_code** – Two-letter postal state code (e.g., CA, NY).
- **state_name** – Full state name.
- **min_bi_per_person** – Minimum bodily injury liability per person (USD).
- **min_bi_per_accident** – Minimum bodily injury liability per accident (USD).
- **min_pd_per_accident** – Minimum property damage liability per accident (USD).
- **notes** – Notes on alternative options, split limits, or special cases.

## Usage Notes

- Values are state-level unless otherwise specified.  
- Always consult original state statutes or regulatory guidance for legal decisions.  
- RU3 provides this data on a best-effort, non-warranted basis.
- 

---

## Related ru3.us Resources

- **Overview:** [Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)  
- **Methodology:** [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)  
- **CSV:** [state-minimum-coverage-limits.csv](/datasets/state-minimum-coverage-limits.csv)  
- **JSON:** [state-minimum-coverage-limits.json](/datasets/state-minimum-coverage-limits.json)

- For a human-readable national comparison view of this dataset, see:  
→ [/minimum-auto-insurance-by-state-table](/minimum-auto-insurance-by-state-table)



<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "State Minimum Auto Liability Coverage Limits",
  "description": "Minimum required auto liability coverage limits by U.S. state.",
  "url": "https://ru3.us/datasets/state-minimum-coverage-limits",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/state-minimum-coverage-limits.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/state-minimum-coverage-limits.json"
    }
  ]
}
</script>
