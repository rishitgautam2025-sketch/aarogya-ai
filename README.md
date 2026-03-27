# Aarogya AI
India's first two-sided health intelligence platform
built for low-income communities.

## Problem
500M Indians lack affordable healthcare access.
₹300-800 consultation fee is a barrier for daily
wage earners. 58% of surveyed users confirm cost
affects their doctor visit decisions.

## Solution
- Symptom triage — AI predicts disease from symptoms
- Doctor discovery — nearest specialists by distance,
  price, rating
- Community health — outbreak alerts for ASHA workers

## How It Works
Patient selects symptoms via checkboxes in Mendix app.
Symptoms are matched against RapidMiner Naive Bayes
model outputs stored in a prediction table. Predicted
disease, risk level, and specialist recommendation
returned in real time. Phase 2 implements live REST
API endpoint.

## Model Performance
- Algorithm: Naive Bayes (best of 205 models)
- Accuracy: 99.3%
- Error Rate: 0.7%
- Stability: ±0.4% standard deviation
- Training: 4,920 examples, 41 diseases, 132 symptoms

## Tech Stack
- Altair RapidMiner AI Studio — predictive modeling
- Mendix Studio Pro — application development

## Datasets
- Disease Symptom Prediction — Pranay Patil (Kaggle)
- Doctor Specialty Recommendation — Ebrahim Elgazar

## Repository Structure
- model/ — RapidMiner exported model (.rmzp)
- data/ — dataset description
- app/ — Mendix screenshots
- report/ — summary report PDF
- pitch/ — presentation deck

## Primary Research
19 respondents, Nagpur, March 2026
- 58% say cost affects doctor visit decisions
- 79% have Googled symptoms before visiting a doctor
- 74% would trust AI to recommend a nearby doctor

## Competition
Data Science Contest — Xpecto'26
IIT Mandi — Supported by Siemens
Deadline: April 4, 2026
```

5. Scroll down → Commit message: `Update README with full project documentation`
6. Click **Commit changes**

---

## Step 7 — Verify Everything Looks Right

Once all files are uploaded, your repo should look like this:
```
aarogya-ai/
├── README.md
├── model/
│   └── Aarogya-AI-NaiveBayes-Model.rmzp
├── data/
│   └── dataset_description.md
├── app/
│   └── screenshots/
│       ├── symptom_checker.png
│       ├── triage_result.png
│       └── asha_dashboard.png
├── report/
│   └── Aarogya_AI_Summary_Report_v2.pdf
└── pitch/
    └── Aarogya_AI_Pitch_Final.pptx
