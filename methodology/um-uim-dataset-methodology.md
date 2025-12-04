---
title: Methodology for the UM/UIM Coverage Dataset
description: How ru3.us compiles, interprets, and maintains the uninsured / underinsured motorist coverage dataset.
layout: default
---

# Methodology for the Uninsured / Underinsured Motorist (UM/UIM) Dataset

The **ru3.us UM/UIM Dataset (Version 2025.01)** is a structured representation of uninsured and underinsured motorist coverage requirements derived from an initial consolidated 2025 reference document.

This page explains **what the dataset does and does not claim to represent**, and how it should be used.

---

## Scope and Intent

The dataset answers two core questions for each jurisdiction:

1. Does the initial reference text explicitly describe **UM or UM/UIM as required**?  
2. Where UM/UIM is described, what are the **stated minimum limits**?

It **does not** attempt to independently re-derive full UM/UIM law for each state. Instead, it:

- Preserves the text as given where requirements are stated.
- Flags all other jurisdictions as `"unknown"` to avoid incorrect inferences.

This makes Version 2025.01 a **partial but honest** representation of UM/UIM requirements.

---

## Fields and Interpretation

Each row includes:

- `state_code` – Two-letter USPS abbreviation.  
- `state_name` – Full state name.  
- `um_uim_required` –  
  - `"yes"` if the initial source text clearly describes UM or UM/UIM minimums as part of the mandatory coverage package.  
  - `"unknown"` if the initial source text does not describe UM/UIM requirements at all.

- `um_uim_limits_text` –  
  A plain-text description of the UM/UIM minimums where specified. Examples include:
  - “$25,000 uninsured/underinsured motorist coverage per person; $50,000 uninsured/underinsured motorist coverage per accident.”
  - “$25,000 uninsured motorist coverage per person; $50,000 uninsured motorist coverage per accident; $25,000 uninsured motorist property damage coverage.”

- `notes` –  
  - Typically: “UM/UIM requirements not specified in initial source text; may be optional, not mandated, or omitted.”  
  - May be expanded in future versions where regulator or statutory sources clarify the status.

---

## Data Sources

Version 2025.01 uses:

1. The same consolidated 2025 state-by-state requirements text that underpins the **minimum liability dataset**, which includes:
   - Liability minimums
   - PIP / MedPay provisions
   - UM/UIM details for some states

2. No additional external sources at this stage.  
   - States where UM/UIM requirements are not described in that text are **not** filled from secondary online sources in this version.

Future versions (e.g., 2025.02 and beyond) may:

- Incorporate regulator or statutory checks for every jurisdiction.
- Convert `"unknown"` entries into `"yes"` / `"no"` with precise limits where appropriate.

---

## Design Choices

Key design decisions:

1. **Avoiding false certainty**  
   Where the source text is silent on UM/UIM, the dataset uses `"unknown"` rather than assuming “not required.”

2. **Text-first representation**  
   Because UM and UIM are frequently grouped and have property damage components in some states, Version 2025.01 stores a single `um_uim_limits_text` field rather than trying to normalize multiple numeric columns prematurely.

3. **Separation from liability dataset**  
   UM/UIM is maintained in its own dataset to:
   - Keep the primary liability dataset simple and consistent.
   - Allow independent evolution as UM/UIM rules are validated and expanded.

---

## Future Enhancements

Planned improvements include:

- Breaking out:
  - `um_bi_per_person`
  - `um_bi_per_accident`
  - `um_pd_per_accident`
  - Separate UIM fields where applicable

- Resolving `"unknown"` entries through:
  - Direct statute review
  - Regulator bulletins
  - Official consumer publications

Each major update will result in a new dataset version with a changelog describing:

- Which states were updated
- How the requirements were validated
- Any structural changes to fields

---

## How to Use This Dataset

You can use this dataset to:

- See which states, per the initial reference, clearly document UM/UIM minimums.
- Compare patterns where UM/UIM is bundled with liability or PIP requirements.
- Build internal tools that **treat `"unknown"` properly as “needs further review.”**

You should **not** use this dataset as a sole, authoritative statement of UM/UIM law in any jurisdiction. Always confirm requirements with:

- State insurance regulators
- Statutes
- Insurers or qualified legal counsel

---

## Related ru3.us Resources

- [UM/UIM Dataset – Overview and Download](/datasets/state-um-uim-minimum-coverage)
- [Minimum Auto Liability Limits Dataset](/datasets/state-minimum-coverage-limits)
- [Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)
- [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)
- [ru3.us Datasets Index](/datasets/)
