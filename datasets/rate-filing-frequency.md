---
title: Auto Insurance Rate Filing Activity by State
description: High-level view of how frequently insurers file rate changes by state.
---

# Auto Insurance Rate Filing Activity by State

**High-level view of how frequently insurers file rate changes by state.**

This dataset is provided as:

- CSV: `/datasets/rate-filing-frequency.csv`  
- JSON: `/datasets/rate-filing-frequency.json`  

## Fields

- **state_code** – Two-letter postal state code.
- **state_name** – Full state name.
- **filings_per_year_estimate** – Approximate number of personal auto rate filings per year.
- **regulatory_approval_type** – prior-approval, file-and-use, or use-and-file.
- **notes** – Additional context on filing processes.

## Usage Notes

- Values are state-level unless otherwise specified.  
- Always consult original state statutes or regulatory guidance for legal decisions.  
- RU3 provides this data on a best-effort, non-warranted basis.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Auto Insurance Rate Filing Activity by State",
  "description": "High-level view of how frequently insurers file rate changes by state.",
  "url": "https://ru3.us/datasets/rate-filing-frequency",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/rate-filing-frequency.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/rate-filing-frequency.json"
    }
  ]
}
</script>
