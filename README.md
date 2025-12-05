# Accounts Payable (AP) Cycle Time Reduction Project

## Process Analysis • Business Intelligence • Excel • BPMN • Miro

---

## Project Overview

This project provides a comprehensive analysis of the organization's Invoice-to-Pay process using 3,000 transactional records. The goal was to identify and quantify the core bottlenecks causing a high average invoice cycle time — which was impacting vendor relationships and financial accruals.

The analysis includes:

- As-Is process mapping and bottleneck identification.  
- Quantitative (Pareto) analysis of delay contribution by responsible actor.  
- Root cause analysis leading to a To-Be automated workflow design (BPMN).  
- Defined business requirements (BRD) for automated implementation.

### Dashboards

While a live dashboard is not shared, the project used visualization to track:
- Invoice Cycle Time Overview  
- Baseline vs. Projected Cycle Time (13 days → < 5 days)  
- Pareto chart showing delay contribution by actor (78% from Approvers)  
- Rework & Exception Metrics  
- Manual touch rate reduction (Projected 65% → < 20%)  
- Escalation Monitoring: Tracking late approval rates vs. escalation triggers  

Final dashboard images and project documentation are available in the project documentation folder.

---

## Data Sources

**Dataset**: Full Invoice Transaction Logs (3,000 records)  
**File**: `invoice_dataset_cleaned.csv`  
**Description**: Timestamps for all invoice status changes — sourced from the organization’s internal ERP and financial databases.

---

## Data Cleaning & Transformation

Processing was performed using Excel to standardize all datasets into a clean analytical model focused on time duration.

Key steps included:

1. Timestamp standardization and validation across all process steps (e.g., Approval Requested vs. Approved Date).  
2. Cycle Time Calculation for each actor and process stage.  
3. Delay Contribution Calculation to perform Pareto Analysis.  
4. Standardization of actor and process stage names.  

**Data Validation**:
- Removed incomplete records without full end-to-end timestamps.  
- Validated the logical consistency of the process flow against the As-Is BPMN.  
- Ensured invoice value and PO data integrity for smart routing analysis.  

---

## Analytical Framework

### KPI Definition
- Average Invoice Cycle Time (Total Days)  
- Process Step Cycle Time (Days per Actor)  
- Delay Percentage Contribution (Pareto Analysis)  

### Data Processing
- Calculated duration metrics using Ms. Excel.  
- Segmented delay by Responsible Actor (Approver 1, Approver 2, AP Team).  
- Correlated long cycle times with specific root causes (e.g., Manual Data Entry, Lack of Escalation).  

### Process Design (BPMN)
- Visualized the inefficient As-Is process.  
- Designed the streamlined To-Be Automated Workflow (eliminating manual steps and enforcing escalation).  

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

- **Approval Process Bottleneck**  
  Finding: Approvers (Stage 1 and 2) account for **78% of the 13-day average cycle time**.  
  Implication: Improvement efforts must target the wait time for human action — not system processing time.

- **Manual Workflow Inefficiency**  
  Finding: The existing fragmented, manual data entry and validation process leads to high rework rates.  
  Implication: A centralized, automated intake and OCR validation system is required to shift the AP team’s focus to high-value exception handling.

- **Solution — Auto-Approval Bypass**  
  Finding: The rigid 2-level approval policy for all invoices (including low-value ones) is a major contributor to the delay.  
  Implication: The To-Be system must implement Auto-Approval for invoices under **$1,000** with a successful 3-Way Match, eliminating the bottleneck without policy risk.

- **Solution — Escalation Logic**  
  Finding: Invoices frequently get stuck with an Approver due to a lack of reminders or defined deadlines.  
  Implication: The To-Be system must implement a **48-hour Timer Event** to automatically trigger a reminder and subsequent escalation to the manager — enforcing accountability.

---

## Deliverables

- Business Requirements Document (BRD)  
- As-Is & To-Be BPMN Diagram (visualizing the automated flow)  
- Project Charter
- Interview Notes

---

## Tools & Technologies

| Tool       | Purpose |
|------------|---------|
| **Excel**    | Data extraction, transformation, and duration calculation, and Pareto visualization |
| **Miro**   | Process mapping (As-Is / To-Be BPMN) and Root Cause Analysis |
| **Notion** | Project documentation and BRD creation |

---

## About the Analyst

Hi, I’m **Syahraini**, transitioning into Business Analysis from an accounting background. I specialize in building clear, executive-ready dashboards and turning complex datasets into practical insights — particularly within financial and operational processes.

---

## Contact

- **LinkedIn**: https://linkedin.com/in/nsyahraini  
- **Portfolio**: https://bit.ly/syahrainiportfolio  
- **Email**: syahraini.nur@outlook.com
