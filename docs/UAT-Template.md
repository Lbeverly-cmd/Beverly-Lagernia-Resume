# Data Validation & UAT Template

**Project:** Quarterly Revenue Audit  
**Analyst:** Lagernia M. Beverly  
**Stakeholder:** Department of Revenue / EOHHS  

## 🧪 Test Case 1: Data Completeness

- **Description:** Ensure all 2026 transaction records were successfully imported.
- **Expected Result:** Count of records in source system matches target database.
- **Status:** [Pass/Fail]

## 🧪 Test Case 2: Join Integrity

- **Description:** Verify that `INNER JOIN` logic did not drop valid taxpayer IDs.
- **Expected Result:** Zero null values in the `TaxID` column post-join.
- **Status:** [Pass/Fail]

## 🧪 Test Case 3: Calculation Accuracy

- **Description:** Manually calculate the average revenue for Category 'A' to verify SQL `AVG()` output.
- **Expected Result:** Manual calculation ($542.10) matches system output.
- **Status:** [Pass/Fail]