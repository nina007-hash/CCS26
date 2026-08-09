OVERVIEW

This repository contains the artifacts for the human-subject study described in the paper "Effects of Explanations on Driver Situation Awareness Under Physical Adversarial Attacks in Automated Driving: A Driving Simulator Study." The artifacts are provided to support the experimental evaluation and statistical analysis made in the manuscript, in accordance with the ACM Artifact Policy. 

The provided Jupyter Notebook allow researchers to conduct all statistics analysis reported in the manuscript regarding driver situation awareness, takeover performance, trust, and mental workload.

================================================================================
ARTIFACT STRUCTURE & ROADMAP

The artifacts are organized as a streamlined, flat directory containing the primary execution script and the documentation. The general layout is as follows:

* `README.txt`: The primary documentation file providing an overview and execution instructions.
* `Statistic_Analysis.ipynb`: The core executable artifact. This Jupyter Notebook contains all the R code necessary to reproduce the statistical analyses. It is cleanly divided into modular cells that correspond exactly to Sections 4.1, 4.2, and 4.3 of the manuscript.
* `Coding.xlsx`: The codebook derived from participants’ responses to the four open-ended questions about their perceptions of explanations and abnormal events across the four attack scenarios, and their insights and suggestions for takeover and attack warnings.
* `Supplementary.pdf`: This supplementary document accompanies the paper. It contains the complete study instruments and statistics results.

================================================================================
ETHICS

To ensure participant privacy and compliance with ethical standards:

Consent: Data was collected with informed consent, specifically allowing for the publication of anonymized results for academic research.

IRB Approval: The study protocol was reviewed and approved by the authors' Institutional Review Board. (Note: IRB Reference numbers are withheld here to maintain double-blind anonymity if required).

================================================================================
SYSTEM REQUIREMENTS & SETUP

No specific hardware is required. The analysis can be run on any standard computer. Recommended Environment: Google Colab (https://colab.research.google.com/)

Upload Statistic_Analysis.ipynb and the three .csv files to a Google Colab environment.

Execute the first cell (%load_ext rpy2.ipython) to initialize the R environment and the second cell to install the required statistical packages
