---
title: Penalties for Auto Insurance Coverage Lapses by State
description: Consequences and reinstatement conditions for lapses in auto coverage.
---

# Penalties for Auto Insurance Coverage Lapses by State

**Consequences and reinstatement conditions for lapses in auto coverage.**

This dataset is provided as:

- CSV: `/datasets/lapse-penalty-rules.csv`  
- JSON: `/datasets/lapse-penalty-rules.json`  

## Fields

- **state_code** – Two-letter postal state code.
- **state_name** – Full state name.
- **license_suspension_possible** – Can a lapse result in license suspension? (yes/no).
- **registration_suspension_possible** – Can a lapse result in registration suspension? (yes/no).
- **sr22_trigger_possible** – Can a lapse trigger SR-22 filing requirements? (yes/no).
- **reinstatement_fee_range** – Typical reinstatement fee range (USD).
- **notes** – Other penalties or conditions.

## Usage Notes

- Values are state-level unless otherwise specified.  
- Always consult original state statutes or regulatory guidance for legal decisions.  
- RU3 provides this data on a best-effort, non-warranted basis.

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "Penalties for Auto Insurance Coverage Lapses by State",
  "description": "Consequences and reinstatement conditions for lapses in auto coverage.",
  "url": "https://ru3.us/datasets/lapse-penalty-rules",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/lapse-penalty-rules.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/lapse-penalty-rules.json"
    }
  ]
}
</script>
