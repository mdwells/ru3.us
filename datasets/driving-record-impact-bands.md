---
title: Illustrative Rate Impacts by Driving Record Scenario
description: Illustrative surcharge ranges and durations for different driving record scenarios by state.
---

# Illustrative Rate Impacts by Driving Record Scenario

**Illustrative surcharge ranges and durations for different driving record scenarios by state.**

This dataset is provided as:

- CSV: `/datasets/driving-record-impact-bands.csv`  
- JSON: `/datasets/driving-record-impact-bands.json`  

## Fields

- **state_code** – Two-letter postal state code.
- **state_name** – Full state name.
- **scenario** – clean, at_fault_accident, dui, speeding_major, etc.
- **surcharge_pct_estimate** – Illustrative surcharge as a percentage of base premium.
- **surcharge_duration_years** – Typical duration over which the surcharge applies.
- **notes** – Source, assumptions, or special rules.

## Usage Notes

- Values are state-level unless otherwise specified.  
- Always consult original state statutes or regulatory guidance for legal decisions.  
- RU3 provides this data on a best-effort, non-warranted basis.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Illustrative Rate Impacts by Driving Record Scenario",
  "description": "Illustrative surcharge ranges and durations for different driving record scenarios by state.",
  "url": "https://ru3.us/datasets/driving-record-impact-bands",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/driving-record-impact-bands.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/driving-record-impact-bands.json"
    }
  ]
}
</script>
