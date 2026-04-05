# Aarogya AI
### India's first two-sided health intelligence platform - built for the last mile

## Demo Video
[Watch Full Project Demo](https://youtu.be/ZwHhtVM8x0w)

---

## Competition
- Event: Data Science Contest - Xpecto'26
- Organizer: IIT Mandi, Supported by Siemens
- Mode: Online, Solo Participation
- Deadline: April 30, 2026

---

## Problem
500 million Indians lack access to affordable healthcare.
The average doctor consultation fee of Rs 300-800 acts as
a barrier for daily wage earners. 58% of our survey
respondents confirmed cost directly affects their doctor
visit decisions. Minor illnesses become emergencies because
people delay diagnosis.

---

## Solution
Aarogya AI serves two users simultaneously:

**For Patients:**
- Enter up to 5 symptoms in plain language
- AI predicts disease with 99.3% accuracy
- Risk level: Red (see doctor today) / Yellow (monitor 3
  days) / Green (home care)
- Nearest specialists shown sorted by distance, price,
  and rating

**For Health Workers:**
- ASHA worker dashboard shows community symptom trends
- Anonymous aggregation detects disease outbreaks early
- Village-level alerts before outbreaks spread

---

## Model Performance
| Metric | Value |
|---|---|
| Algorithm | Naive Bayes (best of 205 models) |
| Accuracy | 99.3% |
| Classification Error | 0.7% |
| Standard Deviation | +/-0.4% |
| Training Examples | 4,920 |
| Diseases Covered | 41 |
| Symptoms Mapped | 132 |
| Validation | Multiple hold-out cross-validation |

### Confusion Matrix Highlights
| Disease | Correct | Accuracy |
|---|---|---|
| Allergy | 38/38 | 100% |
| GERD | 30/30 | 100% |
| Diabetes | 36/36 | 100% |
| Dengue | 35/35 | 100% |
| Fungal Infection | 32/34 | 94% |

---

## Tech Stack
| Tool | Purpose |
|---|---|
| Altair RapidMiner AI Studio | Data preprocessing, feature engineering, predictive modeling |
| Mendix Studio Pro | Patient app, ASHA dashboard, health map |

---

## App Features
- 60 disease-symptom mappings including mental health conditions
- Color coded risk levels (Red/Yellow/Green)
- 3 nearest specialists with distance and consultation fee
- Medical disclaimer on all results
- REST API endpoint for live predictions

---

## Datasets
| Dataset | Source | Details |
|---|---|---|
| Disease Symptom Prediction | Pranay Patil, Kaggle | 4,920 examples, 41 diseases, 132 symptoms, 61,134 downloads |
| Doctor Specialty Recommendation | Ebrahim Elgazar, Kaggle | Maps diseases to correct specialist type |

---

## How It Works
1. Patient enters symptoms in Mendix app
2. Symptoms matched against RapidMiner Naive Bayes model
   outputs stored in prediction table
3. Predicted disease, risk level, and specialist
   recommendation returned in real time
4. If doctor needed, nearest specialists shown with
   distance, fee, and rating
5. Anonymous symptom data aggregated for ASHA worker
   outbreak alerts

Integration note: Current prototype uses RapidMiner-derived
prediction table within Mendix for real-time matching.
Phase 2 implements live REST API endpoint between Mendix
and deployed RapidMiner model.

---

## Primary Research
Survey conducted across Nagpur, March 2026
19 respondents spanning students, salaried workers,
homemakers, and business owners

| Finding | Result |
|---|---|
| Cost affects doctor visit decisions | 58% |
| Have Googled symptoms before visiting doctor | 79% |
| Would trust AI to recommend nearby doctor | 74% |
| Rated AI triage as highly useful (4 or 5 out of 5) | 47% |

Top factors when choosing a doctor: Rating, Specialization,
Proximity

---

## Repository Structure
```
aarogya-ai/
├── README.md
├── model/
│   └── Aarogya-AI-NaiveBayes-Model.rmp
├── data/
│   └── dataset_description.md
├── app/
│   └── screenshots/
├── report/
│   └── Aarogya_AI_Summary_Report_v2.pdf
└── pitch/
    └── Aarogya_AI_Final_v3.pptx
```

---

## Files
- `model/` - Exported RapidMiner Naive Bayes model (.rmp)
- `data/` - Dataset description and source details
- `app/` - Mendix application screenshots
- `report/` - Project summary report (PDF)
- `pitch/` - Presentation deck (11 slides)

---

## Impact
- Reduce unnecessary doctor visits by 40% for non-serious
  conditions
- Early outbreak detection for 500+ villages through
  anonymous symptom aggregation
- Save low-income families Rs 2,000-5,000 annually in
  unnecessary consultation fees
- Scale from village to district to state level

---

## Roadmap
**Phase 1 - Live:** Symptom triage, doctor discovery
**Phase 2 - Next 3 months:** Pre-visit intelligence (symptoms
sent to doctor before appointment), live REST API integration,
follow-up checker
**Phase 3 - 6-12 months:** Voice input in Hindi and Marathi,
health timeline, medicine reminders, offline mode for 2G

---

Built for Bharat. Powered by AI.
Supported by RapidMiner + Mendix.
