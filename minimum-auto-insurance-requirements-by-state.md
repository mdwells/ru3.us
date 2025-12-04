---
title: Minimum Auto Insurance Requirements by State (2025 Edition)
description: State-by-state minimum liability insurance requirements in the U.S., including bodily injury and property damage limits.
layout: default
---

# Minimum Auto Insurance Requirements by State (2025 Edition)

Understanding state minimum auto insurance requirements is essential for evaluating compliance, comparing policies, and understanding the relative cost of auto insurance across states. This guide summarizes the legally mandated minimum **bodily injury** and **property damage** liability requirements for all 50 states and Washington, D.C.

---

## Minimum Liability Requirements Table

Below is a structured comparison based on the **ru3.us minimum liability dataset (Version 2025.01)**.

| State | BI per Person | BI per Accident | PD per Accident |
|-------|---------------|------------------|------------------|
{% for row in site.data.state_minimum_coverage %}
| {{ row.state_name }} | {{ row.min_bi_per_person }} | {{ row.min_bi_per_accident }} | {{ row.min_pd_per_accident }} |
{% endfor %}

---

## What These Numbers Mean

- **Bodily Injury Liability (BI)**  
  Covers medical costs for people injured in an accident you cause.
- **Property Damage Liability (PD)**  
  Covers damage to vehicles, buildings, or other property.

---

## Frequently Asked Questions

### **Which state has the highest minimum auto insurance requirements?**
As of 2025, states with higher-than-average minimums include **Maine**, **Alaska**, **North Carolina**, and **Michigan** (with unique in-state property protection rules).

### **Which states do not require bodily injury liability coverage?**
Florida and New Jersey do not require BI coverage for basic policies. New Hampshire does not require insurance but mandates minimums if you choose to purchase a policy.

### **Where can I download the full dataset?**
- [CSV version](/datasets/state-minimum-coverage-limits.csv)  
- [JSON version](/datasets/state-minimum-coverage-limits.json)

---

## Dataset Source
This summary page is generated from the **ru3.us Minimum Liability Dataset (Version 2025.01)**.

