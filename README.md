DoorDash New Verticals — OOS Analysis

This notebook (ddAnalysis.ipynb) contains the full analysis prepared for the DoorDash New Verticals take-home assignment.

⸻

1) Purpose

The notebook analyzes a one-month sample of DoorDash New Verticals delivery data (Sept 15 – Oct 14, 2022, Cincinnati).
It explores how out-of-stock (OOS) events impact customers, merchants, and dashers by:
	•	Cleaning and standardizing raw delivery + item data
	•	Aggregating to the order level
	•	Computing KPIs (on-time, cancellations, OOS, substitutions, complaints, AOV, CLAT, D2R)
	•	Producing scorecards and charts for Findings 1–3
	•	Running scenario modeling for AOV uplift

⸻

2) Input Data
	•	Dataset: DD Assignment - Dataset.csv (not included in this repo; provided separately for the exercise).
	•	The CSV must be placed in the same working directory as the notebook.
	•	Note: The file has a header row starting on line 2 (header=1 in pandas).

⸻

3) How to Run
	•	Open ddAnalysis.ipynb in Google Colab (recommended) or Jupyter Notebook.
	•	Ensure pandas, numpy, matplotlib, and seaborn are installed.
	•	Upload the dataset and run all cells.
	•	Visuals will render inline.

⸻

4) Outputs

The notebook generates:
	•	Overall Scorecard (KPIs vs. benchmarks)
	•	Store Scorecards (DashMart vs. Grocery)
	•	Charts for Findings 1–3:
	•	OOS vs Complaints
	•	OOS/Subs vs AOV + Complaints
	•	OOS vs CLAT / D2R (Dasher friction)
	•	Scenario modeling for AOV uplift

⸻

5) Notes & Assumptions
	•	All timestamps converted to Eastern Time (ET).
	•	CLAT capped at 120 minutes; D2R capped at 60 minutes (to handle outliers).
	•	Benchmarks/targets are directional ops goals (see report Appendix).
