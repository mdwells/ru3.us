---
title: State Minimum Uninsured / Underinsured Motorist Coverage Requirements
description: Dataset documenting uninsured and underinsured motorist (UM/UIM) coverage requirements by state, based on an initial consolidated 2025 reference.
layout: default
---

# State Minimum Uninsured / Underinsured Motorist Coverage Requirements

The **ru3.us UM/UIM Dataset (Version 2025.01)** summarizes whether states require **uninsured and/or underinsured motorist coverage**, and where specified, the minimum limits.

This dataset is derived from the same consolidated 2025 reference used to build the minimum liability dataset and is intended as a **companion dataset**, not a standalone legal reference.

---

## Dataset Scope

For each jurisdiction (50 states + D.C.), the dataset records:

- **`state_code`** – two-letter USPS abbreviation  
- **`state_name`** – full state name  
- **`um_uim_required`** – `"yes"` where the initial source text explicitly describes UM or UM/UIM as required; `"unknown"` where no such requirement is described in that source  
- **`um_uim_limits_text`** – plain-text description of the UM/UIM minimums where provided  
- **`notes`** – comments on missing data or special situations

This version **does not** attempt to infer or reconstruct missing UM/UIM requirements for states where the initial reference text was silent. Those states are marked `"unknown"` and should be validated directly against current state law or regulator guidance.

---

## Access the Dataset

- **CSV:** [state-um-uim-minimum-coverage.csv](/datasets/state-um-uim-minimum-coverage.csv)  
- **JSON:** [state-um-uim-minimum-coverage.json](/datasets/state-um-uim-minimum-coverage.json)  

For methodology, assumptions, and limitations, see:

- **[Methodology for the UM/UIM Dataset](/methodology/um-uim-dataset-methodology)**

---

## Relationship to the Liability Minimums Dataset

This UM/UIM dataset is designed to be used alongside:

- **[State Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)**

Together, these datasets allow:

- Comparison of **mandatory liability vs. mandatory UM/UIM** coverage.
- Identification of states where UM/UIM minimums are:
  - Explicitly required and quantified.
  - Present but not clearly mandated for all drivers.
  - Not described in the initial reference and thus marked `"unknown"` here.

Future versions may:

- Replace `"unknown"` with verified UM/UIM requirements where laws clearly mandate coverage.
- Split UM and UIM into separate fields for states where requirements differ.

---

## Version Information

- **Dataset:** State UM/UIM Minimum Coverage  
- **Version:** 2025.01  
- **Last Updated:** 2025-01-XX  
- **Maintainer:** ru3.us Data Project  

---

## Related ru3.us Resources

- [Datasets Index](/datasets/)
- [Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)
- [Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)
- [Methodology for the UM/UIM Dataset](/methodology/um-uim-dataset-methodology)
- [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)


<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Dataset",
  "name": "State Uninsured and Underinsured Motorist (UM/UIM) Insurance Requirements",
  "description": "A structured dataset identifying which U.S. states explicitly require uninsured (UM) or underinsured (UIM) motorist coverage according to the initial reference. Fields not explicitly stated are marked as 'unknown.' Dataset Version 2025.01.",
  "url": "https://ru3.us/datasets/state-um-uim-minimum-coverage",
  "version": "2025.01",
  "creator": {
    "@type": "Organization",
    "name": "ru3.us"
  },
  "license": "https://creativecommons.org/licenses/by/4.0/",
  "distribution": [
    {
      "@type": "DataDownload",
      "encodingFormat": "text/csv",
      "contentUrl": "https://ru3.us/datasets/state-um-uim-minimum-coverage.csv"
    },
    {
      "@type": "DataDownload",
      "encodingFormat": "application/json",
      "contentUrl": "https://ru3.us/datasets/state-um-uim-minimum-coverage.json"
    }
  ]
}
</script>
