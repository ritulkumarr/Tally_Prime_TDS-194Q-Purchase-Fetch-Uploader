# TDS-194Q-Purchase-Fetch-Uploader
Excel Power Query automation to fetch, clean, and consolidate vendor-wise purchase and GST data from multiple files for accurate TDS compliance under Section 194Q.

**Overview**

This project is an Excel Power Query automation designed to fetch, clean, consolidate, and summarize vendor-wise purchase data from multiple Excel files to support TDS compliance under Section 194Q of the Income Tax Act.

It eliminates manual consolidation work and reduces errors in identifying 194Q-applicable purchase values (excluding GST), especially in high-volume vendor scenarios.

**Problem Statement**

Organizations often receive purchase data in multiple Excel files with inconsistent formats, headers, and ledger structures.
Manual consolidation for 194Q threshold checking (₹50 lakh) is time-consuming and error-prone.

This tool solves that problem through fully dynamic Power Query logic.

**Key Features**

Dynamic folder-based file loading (no hardcoded paths)

Automatically ignores hidden/system files

Processes multiple Excel files and sheets

Detects headers dynamically (DATE / PARTICULARS)

Removes Grand Total rows to prevent double counting

Normalizes vendor names from file names

**Dynamically identifies:**

Purchase ledgers

GST input ledgers

Unpivots and aggregates data safely

Produces vendor-wise consolidated purchase & GST totals

Ready for 194Q applicability analysis

**Business Logic (194Q Focus)**

Purchase value is consolidated vendor-wise

GST amounts are identified separately

Helps ensure GST is excluded while checking the ₹50 lakh threshold

Scalable for large datasets and multiple vendors

**How It Works (High-Level Flow)**

User provides a folder path via Excel named range FolderPath

All Excel files in the folder are loaded

Headers are detected dynamically

Purchase and GST ledgers are identified using naming logic

Data is unpivoted and cleaned

Vendor-wise totals are calculated

Final consolidated output is generated

**Technical Highlights**

Built using Power Query (M Language)

No hardcoded sheet names or column positions

Works across inconsistent vendor formats

Error-tolerant header promotion and expansion logic

**Tools & Technologies**

Microsoft Excel

Power Query (M)

Tally-compatible ledger structure

**Use Cases**

Finance & Accounts teams

TDS compliance professionals

Companies with high purchase volume

Tally users preparing 194Q calculations

Freelancers automating finance workflows

**Output**

Final output includes:

Vendor Name

Purchase Ledger

Total Purchase Amount

Total GST Amount

This output can be directly used for:

194Q threshold verification

Internal audits

Further TDS calculation workflows

**Project Status**

✔ Active
✔ Functional
✔ Scalable for production use

**Author**

Ritul Kumar
Finance Executive | Excel & Power Query Automation
Specialized in GST, TDS, and Finance Process Automation

**License**

This project is licensed under the MIT License.
