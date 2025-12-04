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
