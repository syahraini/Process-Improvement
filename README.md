# Accounts Payable (AP) Workflow Automation Project

## Process Analysis • Business Intelligence • Excel • BPMN • Miro

---

## Project Overview

This project provides a comprehensive, data-driven analysis of the organization's critical Invoice-to-Pay process, utilizing 15,350 transactional records. The goal was to conclusively identify and quantify the systemic bottlenecks causing the catastrophic 13-day average invoice cycle time — a failure impacting vendor relationships, financial accruals, and overall organizational compliance (2.22% SLA).

The analysis and design deliverables include:
- Rigorously validated As-Is process mapping and bottleneck quantification (13 days of passive waiting).
- Quantitative (Pareto) and Qualitative (5 Whys, Fishbone) Root Cause Analysis.
- Defined To-Be Automated Workflow Design (BPMN) to eliminate manual steps and enforce accountability.
- Finalized Business Requirements Document (BRD v1.0) with MoSCoW prioritization and SMART success criteria.

## Data Sources

**Dataset**: Full Invoice Transaction Logs (15,350 records)  
**File**: `invoice_dataset_cleaned.csv`  
**Description**: Timestamps for all invoice status changes — sourced from the organization’s internal ERP and financial databases.

---

## Data Cleaning & Transformation

Processing was performed using Excel to standardize all datasets into a clean analytical model focused on time duration.
Key steps included:
- Timestamp standardization and validation across all process steps (e.g., Approval Requested vs. Approved Date).
- Cycle Time Calculation for each actor and process stage (identifying the 7.53-day bottleneck).
- Delay Contribution Calculation to perform Pareto Analysis.
- Data Validation: Removed incomplete records without full end-to-end timestamps.

---

## Analytical Framework

### KPI Definition
- Average Invoice Cycle Time (Total Days)
- Process Step Cycle Time (Days per Actor)
- Delay Percentage Contribution (Pareto Analysis)
- Rework Rate & SLA Compliance (2.22%) 

### Data Processing
- Calculated duration metrics using Ms. Excel.
- Segmented delay by Responsible Actor (Approver 1, Approver 2, AP Team).
- Correlated long cycle times with systemic root causes using 5 Whys and Fishbone Analysis.
- Prioritized all solutions using MoSCoW and defined project success with SMART Criteria.

### Process Design (BPMN)
- Visualized the inefficient As-Is process.
- Designed the streamlined To-Be Automated Workflow (eliminating manual steps and enforcing automated escalation).  

---

## Scope Definition

| In-Scope ✔ | Out-of-Scope ✘ |
|-----------|----------------|
| Invoice Cycle Time Analysis | Forecasting future volume |
| Quantitative Bottleneck Identification | Vendor compliance cost analysis |
| To-Be Automated Process Design (BPMN) | Employee expense report process |
| Business Requirements Document (BRD) | Technical architecture of the new ERP |

---

## Key Insights & Findings

- **Approval Process Bottleneck (The Passive Wait)**  
  Finding: Approvers (Stage 1 and 2) account for 78% of the 13-day average cycle time.
  Implication: The core problem is passive waiting (not processing speed). The solution must implement a hard deadline and automated escalation.

- **Intake Quality Failure**  
  Finding: Unstructured intake channels (Email, WA) are the source of 45.57% of all rework.
  Implication: A centralized, mandatory intake portal with tollgate validation is required to eliminate low-value exception handling and reduce the 14.12% rework rate.

- **Solution — Escalation Logic**  
  Finding: Invoices frequently get stuck with an Approver due to a lack of defined deadlines.  
  Implication: The To-Be system must implement a 72-hour Timer Event to automatically trigger a reminder and subsequent escalation to the manager, enforcing accountability and eliminating the 13-day delay.

- **Solution — Auto-Approval Bypass**  
  Finding: The rigid 2-level approval policy for all invoices (including low-value ones) is a major contributor to the delay.
  Implication: The To-Be system implements Auto-Approval for invoices under < $1,000 with a successful 3-Way Match, leveraging automation to achieve a Quick Win.
  
---

## Deliverables

- Project Charter
- As-Is BPMN Diagram (Miro)
- Data Analysis Report (cycle time, bottlenecks, SLA, Pareto)
- Pain Points & Root Cause Summary
- To-Be BPMN Diagram (Miro)
- BRD (requirements + acceptance criteria)
- Executive Summary

---

## Tools & Technologies

| Tool       | Purpose |
|------------|---------|
| **Excel**  | Data extraction, transformation, and duration calculation, and Pareto visualization |
| **Miro**   | Process mapping (As-Is / To-Be BPMN) and Root Cause Analysis |
| **Notion** | Project documentation and BRD creation |
| **Canva** | Presentation |

---

## About the Analyst

Hi, I’m **Syahraini**, transitioning into Business Analysis from an accounting background. I specialize in building clear, executive-ready dashboards and turning complex datasets into practical insights — particularly within financial and operational processes.

---

## Contact

- **LinkedIn**: https://linkedin.com/in/nsyahraini  
- **Portfolio**: https://bit.ly/syahrainiportfolio  
- **Email**: syahraini.nur@outlook.com
