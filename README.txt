OVERVIEW

This repository contains the anonymized dataset collected from the human-subject study described in the paper "Effects of Explanations on Driver Situation Awareness Under Physical Adversarial Attacks in Automated Driving: A Driving Simulator Study." The artifact is provided to support the experimental evaluation and statistical analysis made in the manuscript, in accordance with the ACM Artifact Policy.

The provided Jupyter Notebook and cleaned CSV datasets allow researchers to perfectly reproduce all statistics analysis reported in the manuscript regarding Driver Situation Awareness, Takeover Performance, Trust, and Mental Workload. The codebook is for qualitative analysis including the summary of the frequency of each code in sub-sheets.

================================================================================
ARTIFACT STRUCTURE & ROADMAP

The artifact is organized as a streamlined, flat directory containing the primary execution script, the supporting datasets, and the documentation. The general layout is as follows:

README.txt: The primary documentation file providing an overview, data dictionary, and execution instructions.

Statistic_Analysis.ipynb: The core executable artifact. This Jupyter Notebook contains all the R code necessary to reproduce the statistical analyses. It is cleanly divided into modular cells that correspond exactly to Sections 4.1, 4.2, and 4.3 of the manuscript.

data_for_driver_SA.csv: The granular dataset including driver overall and three levels SA.

data_for_takeover_performance.csv: The performance dataset including Longitudinal and Lateral Reaction Times..

data_for_trust&workload.csv: The aggregated dataset used to evaluate Trust and Mental Workload.

codebook.xlsx: The coded data used to evaluate subjective open-ended questions responses.

================================================================================
DATA & ETHICS

To ensure participant privacy and compliance with ethical standards:

Anonymization: All Personally Identifiable Information has been stripped from this dataset. Participants are identified solely by randomized IDs (1-32).

Consent: Data was collected with informed consent, specifically allowing for the publication of anonymized results for academic research.

IRB Approval: The study protocol was reviewed and approved by the authors' Institutional Review Board. (Note: IRB Reference numbers are withheld here to maintain double-blind anonymity if required).

================================================================================
DATA DICTIONARY

data_for_driver_SA.csv & data_for_takeover_performance.csv: Contain the granular data for all 32 participants across the physical adversarial attacks.

Columns:
Participant: Unique anonymized identifier (1-32).
Group: Experimental condition assignment (0 = Without Explanation [Control], 1 = With Explanation [Experimental]).
Level: The three levels of Situation Awareness (1 = Perception, 2 = Comprehension, 3 = Projection).
Attack: Coded ID for the specific physical adversarial attack scenario (1 = Stop Sign, 2 = Vehicle, 3 = Pedestrian, 4 = Lane Markings).
Reliability: System reliability state (0 = Low Reliability, 1 = High Reliability).
Order: Order in which the attacks were experienced (1st to 4th) to account for ordering effects.
Initial_level / Level_SA: Situation Awareness score for the specific SA level (Binary: 0 or 1).
Initial_SA / Overall_SA: Cumulative Situation Awareness score for the trial (Scale: 0 to 3).
SA_change: Calculated change in the Overall SA score (Scale: -3 to 3).
RT_Longitudinal: Reaction time in seconds for longitudinal control takeover (Braking/Accelerating).
RT_Lateral: Reaction time in seconds for lateral control takeover (Steering).

data_for_trust&workload.csv: Contains the Trust and Mental Workload Surveys responses for each drive.

Columns:
Participant_ID: Unique anonymized identifier (1-32).
Group: Experimental condition assignment (0 = Without Explanation, 1 = With Explanation).
Reliability: System reliability state of the drive (0 = Low Reliability, 1 = High Reliability).
Drive_order: Order of the formal drive (1st or 2nd) to account for learning/fatigue effects.
Trust: Subjective trust score derived from the post-drive survey (Scale: 1-7).
Mental_Workload: NASA-TLX workload score derived from the post-drive survey (Scale: 1-7).

codebook.xlsx: Contains the frequency of each code for each participant's answers for open-ended questions in the sub-sheets.

================================================================================
SYSTEM REQUIREMENTS & SETUP

No specific hardware is required. The analysis can be run on any standard computer. Recommended Environment: Google Colab (https://colab.research.google.com/)

Upload Statistic_Analysis.ipynb and the three .csv files to a Google Colab environment.

Execute the first cell (%load_ext rpy2.ipython) to initialize the R environment and the second cell to install the required statistical packages

================================================================================
USAGE & EXECUTION

To reproduce the paper's findings, run the notebook cells sequentially to reproduce mapped section results.