---
title: No-Fault Auto Insurance
description: Definition of no-fault auto insurance and how it relates to PIP and state minimum requirements.
layout: default
---

# No-Fault Auto Insurance

In a **no-fault auto insurance system**, each driver’s own policy pays for **their injuries** after a crash, regardless of who caused it.

Key characteristics:

- Requires **Personal Injury Protection (PIP)** or similar benefits  
- Limits certain lawsuits for injuries against at-fault drivers  
- Still often uses fault-based rules for **property damage**

---

## No-Fault in the ru3.us Project

The **PIP / No-Fault Dataset (Version 2025.01)** records:

- States with clearly required PIP coverage  
- Core PIP medical amounts  
- Descriptive PIP text  

However, in this version:

- `no_fault_status` is set to `"unknown"` for all states, because the project avoids guessing about regime classification without explicit statutory/regulator sourcing.

Dataset access:

- Documentation → [/datasets/state-pip-no-fault-coverage](/datasets/state-pip-no-fault-coverage)  
- CSV → [/datasets/state-pip-no-fault-coverage.csv](/datasets/state-pip-no-fault-coverage.csv)  
- JSON → [/datasets/state-pip-no-fault-coverage.json](/datasets/state-pip-no-fault-coverage.json)

---

## Example No-Fault States

Based on widely understood structures (not encoded as `no_fault_status` yet), key no-fault states include:

- Florida  
- New York  
- Michigan  
- New Jersey, Massachusetts, and others

See their detailed pages:

- [/state/florida-minimum-auto-insurance](/state/florida-minimum-auto-insurance)  
- [/state/new-york-minimum-auto-insurance](/state/new-york-minimum-auto-insurance)  
- [/state/michigan-minimum-auto-insurance](/state/michigan-minimum-auto-insurance)

---

## Related Terms

- [Personal Injury Protection (PIP)](/glossary/personal-injury-protection-pip)  
- [Tort State](/glossary/tort-state)  
- [Choice No-Fault State](/glossary/choice-no-fault-state)
