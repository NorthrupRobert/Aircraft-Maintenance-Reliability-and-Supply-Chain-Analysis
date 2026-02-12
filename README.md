<p align="center">
  <img src="/assets/vectra logo white.png" width="250">
</p>

# Delta 737-800 Maintenance, Reliability, and Supply Chain Analysis
### *SUBTITLE HERE*

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active-brightgreen"></a>
  <img src="https://img.shields.io/badge/Focus-Aerospace-lightblue"></a>
  <img src="https://img.shields.io/badge/Database/Querying-PostgreSQL-white"></a>
  <img src="https://img.shields.io/badge/Analysis-Python-gold"></a>
  <img src="https://img.shields.io/badge/Visualization-Tableau-hotpink"></a>
  <img src="https://img.shields.io/badge/Updated-Feb%202026-lightgrey"></a>
</p>

---

## AUTHOR
**Robb Northrup**

Data Analytics | Aerospace | Community Impact

**Date** Feb 10, 2026 - PRESENT

<p align="center">
  <a href="https://linkedin.com/in/robb-northrup-463867382"><img src="https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin"></a>
  <a href="https://github.com/NorthrupRobert/portfolio"><img src="https://img.shields.io/badge/GitHub-Portfolio-black?style=for-the-badge&logo=github"></a>
  <a href="mailto:robbnorthrup@outlook.com"><img src="https://img.shields.io/badge/Email-Contact-green?style=for-the-badge&logo=gmail"></a>
</p>

---

## TABLE OF CONTENTS
- [Executive_Summary](#executive-summary)
- [Background](#background)
- [Data_Structure_Overview](#data-structure-overview)
- [Insights_Deep_Dive](#insights-deep-dive)
- [Recommended_Actions](#recommended-actions)

---

## EXECUTIVE SUMMARY
VECTRA SPACE (Fictional Airline) has been operating for the past 150 years, providing top of the line service . . .
“This project simulates the maintenance and operational challenges of a Boeing 737‑800 fleet operated by a mid‑size U.S. airline.
FAA Service Difficulty Reports (SDR) are used as a proxy for real-world maintenance events.”

### Problem Statement
**How can an aviation organization reduce unscheduled maintenance events and their operational and supply chain impacts by identifying high‑risk components, predicting failures, and optimizing parts availability?**

### Project Aim
**LIST HERE**

### Dashboards
**DASHBOARDS HERE**

### Key Findings
**LIST HERE**

<div style="font-size: 0.85em">
**Resources**

- Click here to access the Dashboards and Project Data.
- Click here to access the [Performance Executive Summary]
- Click here to access the [Impact Analysis Slide Deck]

</div>

---

## BACKGROUND
**BACKGROUND HERE**

---

## DATA STRUCTURE OVERVIEW

### Assumptions and Synthetic Logic
This project uses FAA Service Difficulty Reports (SDRs) as the authoritative source for real maintenance events, failure modes, JASC codes, and component descriptions. Because SDRs only capture failures and discrepancies—not the full aircraft bill of materials—the supply‑chain layer (unit cost, lead time, supplier assignment, stocking levels) is intentionally synthetic. All synthetic values are grounded in real aviation patterns: JASC/ATA chapter drives criticality and lead‑time behavior, part names and conditions influence cost heuristics, and failure frequency from SDRs determines stocking logic. The goal is not to recreate Boeing’s proprietary ERP, but to build a realistic, explainable model that mirrors how reliability and supply‑chain analysts reason about parts when full ERP data is unavailable.

### How the System Works
The pipeline ingests the SDR composite file, normalizes Part* and Component* fields, and merges them into a unified “parts universe” representing all components that appeared in real maintenance events. From there, the system generates a parts master table with synthetic but aviation‑grounded attributes (cost, lead time, criticality, supplier). A supplier table is created with performance metrics, and an inventory table is derived by combining failure frequency, criticality, cost, and lead‑time heuristics. These tables form a miniature but coherent maintenance‑and‑supply‑chain ecosystem that can be loaded into SQL for analysis and visualized in Tableau for reliability and logistics insights.

### AI‑Generated Components
The synthetic supply‑chain attributes and the logic that produces them were developed with the assistance of an AI system. The AI did not invent real proprietary data; instead, it generated structured, explainable heuristics based on aviation maintenance conventions, ATA/JASC patterns, and reliability engineering principles. All synthetic elements are clearly separated from the real SDR data, and the methodology is fully documented so that assumptions can be inspected, challenged, or extended. This approach allows the project to remain realistic, transparent, and professionally defensible while still enabling end‑to‑end analytics across maintenance, reliability, and supply‑chain domains.

### Data Sources

### Why Normalization Was Needed

### Data Model
The ERD below shows how Events, Members, Officers, and Participation connect to support many‑to‑many relationships essential for engagement and continuity analysis.

**ERD IMAGE HERE**

---

## INSIGHTS DEEP DIVE
### 1. INSIGHT
ONE SENTENCE OVERVIEW
- SUPPORTING STATEMENT 1
- SUPPORTING STATEMENT 2

### 2. INSIGHT
ONE SENTENCE OVERVIEW
- SUPPORTING STATEMENT 1
- SUPPORTING STATEMENT 2

---

## RECOMMENDED ACTIONS
### 1. RECOMMENDATION
- DETAIL 1
- DETAIL 2

### 2. RECOMMENDATION
- DETAIL 1
- DETAIL 2
