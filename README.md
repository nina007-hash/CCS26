# CCS26
# Human Subject Study Data

## Overview
This repository contains the anonymized dataset collected from the human-subject study described in the submission **"Effects of Explanations on Driver Situation Awareness Under Physical Adversarial Attacks in Automated Driving: A Driving Simulator Study**. These artifacts are provided to support the experimental evaluation and statistical analysis made in the manuscript, in accordance with the conference's Artifact Policy.

## Data & Ethics
To ensure participant privacy and compliance with ethical standards:
* **Anonymization:** All Personally Identifiable Information has been stripped from this dataset. Participants are identified solely by randomized IDs.
* **Consent:** Data was collected with informed consent, specifically allowing for the publication of anonymized results for academic research.
* **IRB Approval:** The study protocol was reviewed and approved by the authors' Institutional Review Board. (IRB Reference numbers are withheld to maintain double-blind anonymity).

## Repository Structure
**Note on File Formats:**
While `data_by_attack.csv` and `data_by_reliability.csv` are provided in standard CSV format for easy machine parsing, `codebook.xlsx` is provided as an Excel file. This is because the codebook utilizes **merged cells and hierarchical headers** to group related survey questions and response categories visually. Converting this file to CSV would strip this formatting and make the coding schema difficult to interpret.

The data is organized as follows:

```text
/
## Repository Structure
The data is organized as follows:

```text
/
├── data_by_attack.csv       # Dataset for SA (overall, each level), RT for longitudinal ontrol, and RT for lateral control by attack objects
├── data_by_reliability.csv  # Dataset for SA, RT for longitudinal control, RT for lateral control, trust and mental workload assessments by ADS reliability
├── codebook.xlsx            # Anonymized post-study survey codes
├── data_dictionary.md       # Definitions of column headers and metrics
└── README.md                # This file
