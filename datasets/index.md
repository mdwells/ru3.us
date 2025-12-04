---
title: ru3.us Datasets – Auto Insurance Requirements and Structured State Data
description: Index of all structured datasets published by ru3.us, including state minimum auto liability limits and supporting documentation.
layout: default
---

# ru3.us Datasets

The **ru3.us dataset library** provides structured, documented, and machine-readable information related to **U.S. auto insurance requirements**.  
All datasets include:

- **Clear schemas**
- **Stable versioning**
- **CSV and JSON formats**
- **Methodology and sourcing details**
- **Human-readable reference pages**

This hub lists all currently published datasets and supporting resources.

---

## 📌 Minimum Auto Liability Limits (Dataset Version 2025.01)

This dataset contains the **state-mandated minimum auto liability insurance limits** for:

- All 50 U.S. states  
- The District of Columbia  

The dataset includes:

| Field | Description |
|-------|-------------|
| `state_code` | Two-letter USPS abbreviation |
| `state_name` | Full state name |
| `min_bi_per_person` | Bodily injury liability per person |
| `min_bi_per_accident` | Bodily injury liability per accident |
| `min_pd_per_accident` | Property damage liability per accident |
| `notes` | Special cases or explanatory details |

### Access the Dataset

- **Dataset documentation:**  
  ➜ [State Minimum Auto Liability Limits – Documentation](/datasets/state-minimum-coverage-limits)

- **Download the dataset:**  
  - **CSV:** [state-minimum-coverage-limits.csv](/datasets/state-minimum-coverage-limits.csv)  
  - **JSON:** [state-minimum-coverage-limits.json](/datasets/state-minimum-coverage-limits.json)

- **Methodology and sourcing:**  
  ➜ [Methodology for the Minimum Auto Liability Dataset](/methodology/minimum-liability-dataset-methodology)

---

## 🛡 Uninsured / Underinsured Motorist Coverage Dataset (Version 2025.01)

This dataset captures where the initial 2025 reference explicitly describes **uninsured and underinsured motorist (UM/UIM) coverage requirements** and records those limits as text.

Because the underlying source is incomplete on UM/UIM, many states are conservatively marked as `"unknown"` rather than assumed to have no requirement.

### Access the Dataset

- **Dataset documentation:**  
  ➜ [UM/UIM Coverage Requirements – Documentation](/datasets/state-um-uim-minimum-coverage)

- **Download the dataset:**  
  - **CSV:** [state-um-uim-minimum-coverage.csv](/datasets/state-um-uim-minimum-coverage.csv)  
  - **JSON:** [state-um-uim-minimum-coverage.json](/datasets/state-um-uim-minimum-coverage.json)

- **Methodology:**  
  ➜ [Methodology for the UM/UIM Dataset](/methodology/um-uim-dataset-methodology)

---

## 🧾 Personal Injury Protection (PIP) / No-Fault Dataset (Version 2025.01)

This dataset captures where an initial 2025 reference explicitly describes **personal injury protection (PIP)** requirements and records the core PIP medical amount and descriptive text. It does **not** yet classify states as tort vs. no-fault; all entries have `no_fault_status = "unknown"` in Version 2025.01.

### Access the Dataset

- **Dataset documentation:**  
  ➜ [PIP / No-Fault Coverage Dataset](/datasets/state-pip-no-fault-coverage)

- **Download the dataset:**  
  - **CSV:** [state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
  - **JSON:** [state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)

- **Methodology:**  
  ➜ [Methodology for the PIP / No-Fault Dataset](/methodology/pip-no-fault-dataset-methodology)

---

## 📚 Reference Pages Built from This Dataset

These pages provide narrative explanations and state-specific context using the structured data.

### Overview

- **[Minimum Auto Insurance Requirements by State (2025 Edition)](/minimum-auto-insurance-requirements-by-state)**  
  A full table of state minimums, plain-language explanations, and download links.

### Featured State Pages

- [California](/state/california-minimum-auto-insurance)  
- [Texas](/state/texas-minimum-auto-insurance)  
- [Florida](/state/florida-minimum-auto-insurance)  
- [New York](/state/new-york-minimum-auto-insurance)  
- [Michigan](/state/michigan-minimum-auto-insurance)  

More will be added as state-level coverage expands.

---

## 🔧 Dataset Roadmap

ru3.us plans to publish additional structured datasets, including:

- **UM/UIM minimum coverage requirements by state**  
- **PIP and no-fault rules by state**  
- **Financial responsibility laws and alternatives**  
- **State-level insurance regulatory structures**  
- **Historical changes to minimum liability limits**

Each dataset will follow the same conventions:

- Versioned  
- CSV + JSON formats  
- Documented methodology  
- State-level detail  
- Human-readable companion pages  

---

## 📄 Notes and Licensing

- All datasets are free to reference, quote, or use with attribution.  
- Data is provided “as is” and is periodically updated as statutes and regulations change.  
- This site does not provide legal advice; verify requirements with state regulators or insurers.

---

## 🔗 Related ru3.us Resources

- [Homepage](/)
- [Minimum Auto Insurance Requirements by State](/minimum-auto-insurance-requirements-by-state)
- [Dataset Documentation](/datasets/state-minimum-coverage-limits)
- [Methodology](/methodology/minimum-liability-dataset-methodology)
