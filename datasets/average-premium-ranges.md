---
title: Estimated Annual Auto Insurance Premium Ranges by State
description: Indicative annual premium ranges for minimum and full coverage by state.
---

# Estimated Annual Auto Insurance Premium Ranges by State

**Indicative annual premium ranges for minimum and full coverage by state.**

This dataset is provided as:

- CSV: `/datasets/average-premium-ranges.csv`  
- JSON: `/datasets/average-premium-ranges.json`  

## Fields

- **state_code** – Two-letter postal state code.
- **state_name** – Full state name.
- **data_year** – Year of the estimate (YYYY).
- **coverage_level** – minimum or full.
- **annual_premium_low** – Lower bound of estimated annual premium (USD).
- **annual_premium_high** – Upper bound of estimated annual premium (USD).
- **source** – Primary data or synthesis source.

## Usage Notes

- Values are state-level unless otherwise specified.  
- Always consult original state statutes or regulatory guidance for legal decisions.  
- RU3 provides this data on a best-effort, non-warranted basis.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Estimated Annual Auto Insurance Premium Ranges by State",
  "description": "Indicative annual premium ranges for minimum and full coverage by state.",
  "url": "https://ru3.us/datasets/average-premium-ranges",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/average-premium-ranges.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/average-premium-ranges.json"
    }
  ]
}
</script>
