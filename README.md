# Aarogya AI
### India's first two-sided health intelligence 
platform - built for the last mile

## Demo Video
[Watch Full Project Demo](https://youtu.be/AOo-Iz3tVVI)

---

## Competition
- Event: Data Science Contest - Xpecto'26
- Organizer: IIT Mandi, Supported by Siemens
- Mode: Online, Solo Participation
- Deadline: April 30, 2026

---

## Problem
500 million Indians lack access to affordable 
healthcare. The average doctor consultation fee of 
Rs 300-800 acts as a barrier for daily wage earners. 
58% of our survey respondents confirmed cost directly 
affects their doctor visit decisions. Minor illnesses 
become emergencies because people delay diagnosis.

---

## Solution
Aarogya AI serves two users simultaneously:

**For Patients:**
- Select symptoms via structured interface
- AI predicts disease with 99.3% accuracy
- Dynamic risk triage: Red (see doctor today) / 
  Yellow (monitor 3 days) / Green (home care)
- Nearest specialists shown with distance, 
  consultation fee, and rating
- Medical disclaimer on all results

**For Health Workers:**
- ASHA worker dashboard shows community symptom trends
- Anonymous aggregation detects disease outbreaks early
- Village-level alerts before outbreaks spread

---

## App Features
- 60 disease-symptom mappings including mental 
  health conditions
- Color coded risk levels (Red/Yellow/Green)
- Emergency escalation - critical symptoms like 
  chest pain immediately flag HIGH risk
- 3 nearest specialists with distance and 
  consultation fee
- REST API endpoint for live predictions
- Geoapify Places API integrated for real-time 
  doctor discovery (Phase 2 - live GPS location)

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

Note: 99.3% accuracy reflects performance on a 
clean structured Kaggle dataset. Real-world 
performance with noisy input will be validated 
in Phase 2 field testing.

---

## Tech Stack
| Tool | Purpose |
|---|---|
| Altair RapidMiner AI Studio | Data preprocessing, feature engineering, predictive modeling |
| Mendix Studio Pro | Patient app, ASHA dashboard, health map |
| Geoapify Places API | Real-time doctor and clinic discovery |

---

## Datasets
| Dataset | Source | Details |
|---|---|---|
| Disease Symptom Prediction | Pranay Patil, Kaggle | 4,920 examples, 41 diseases, 132 symptoms, 61,134 downloads |
| Doctor Specialty Recommendation | Ebrahim Elgazar, Kaggle | Maps diseases to correct specialist type |

---

## How It Works
1. Patient selects symptoms in Mendix app
2. Symptoms matched against RapidMiner Naive Bayes 
   model outputs stored in prediction table
3. Predicted disease, risk level, and specialist 
   recommendation returned in real time
4. Nearest specialists shown with distance, fee, 
   and rating
5. Anonymous symptom data aggregated for ASHA 
   worker outbreak alerts

Integration note: Current prototype uses 
RapidMiner-derived prediction table within Mendix 
for real-time matching. Phase 2 implements live 
REST API endpoint between Mendix and deployed 
RapidMiner model.

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
| Rated AI triage as highly useful | 47% |

---

## Repository Structure
aarogya-ai/
- README.md
- model/ - Exported RapidMiner Naive Bayes model
- data/ - Dataset description and source details
- app/ - Mendix application screenshots
- report/ - Project summary report (PDF)
- pitch/ - Presentation deck

---

## Impact
- Reduce unnecessary doctor visits for non-serious 
  conditions
- Early outbreak detection for 500+ villages through 
  anonymous symptom aggregation
- Save low-income families Rs 2,000-5,000 annually
- Scale from village to district to state level

---

## Roadmap
Phase 1 - Live: Symptom triage, doctor discovery, 
color coded risk levels
Phase 2 - Next 3 months: Live GPS location, live 
RapidMiner API endpoint, pre-visit intelligence
Phase 3 - 6-12 months: Voice input in Hindi, 
Marathi, and Pahari, health timeline, offline 
mode for 2G areas

---

Built for Bharat. Powered by AI.
Supported by RapidMiner + Mendix.# Aarogya AI
### India's first two-sided health intelligence 
platform - built for the last mile

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
500 million Indians lack access to affordable 
healthcare. The average doctor consultation fee of 
Rs 300-800 acts as a barrier for daily wage earners. 
58% of our survey respondents confirmed cost directly 
affects their doctor visit decisions. Minor illnesses 
become emergencies because people delay diagnosis.

---

## Solution
Aarogya AI serves two users simultaneously:

**For Patients:**
- Select symptoms via structured interface
- AI predicts disease with 99.3% accuracy
- Dynamic risk triage: Red (see doctor today) / 
  Yellow (monitor 3 days) / Green (home care)
- Nearest specialists shown with distance, 
  consultation fee, and rating
- Medical disclaimer on all results

**For Health Workers:**
- ASHA worker dashboard shows community symptom trends
- Anonymous aggregation detects disease outbreaks early
- Village-level alerts before outbreaks spread

---

## App Features
- 60 disease-symptom mappings including mental 
  health conditions
- Color coded risk levels (Red/Yellow/Green)
- Emergency escalation - critical symptoms like 
  chest pain immediately flag HIGH risk
- 3 nearest specialists with distance and 
  consultation fee
- REST API endpoint for live predictions
- Geoapify Places API integrated for real-time 
  doctor discovery (Phase 2 - live GPS location)

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

Note: 99.3% accuracy reflects performance on a 
clean structured Kaggle dataset. Real-world 
performance with noisy input will be validated 
in Phase 2 field testing.

---

## Tech Stack
| Tool | Purpose |
|---|---|
| Altair RapidMiner AI Studio | Data preprocessing, feature engineering, predictive modeling |
| Mendix Studio Pro | Patient app, ASHA dashboard, health map |
| Geoapify Places API | Real-time doctor and clinic discovery |

---

## Datasets
| Dataset | Source | Details |
|---|---|---|
| Disease Symptom Prediction | Pranay Patil, Kaggle | 4,920 examples, 41 diseases, 132 symptoms, 61,134 downloads |
| Doctor Specialty Recommendation | Ebrahim Elgazar, Kaggle | Maps diseases to correct specialist type |

---

## How It Works
1. Patient selects symptoms in Mendix app
2. Symptoms matched against RapidMiner Naive Bayes 
   model outputs stored in prediction table
3. Predicted disease, risk level, and specialist 
   recommendation returned in real time
4. Nearest specialists shown with distance, fee, 
   and rating
5. Anonymous symptom data aggregated for ASHA 
   worker outbreak alerts

Integration note: Current prototype uses 
RapidMiner-derived prediction table within Mendix 
for real-time matching. Phase 2 implements live 
REST API endpoint between Mendix and deployed 
RapidMiner model.

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
| Rated AI triage as highly useful | 47% |

---

## Repository Structure
aarogya-ai/
- README.md
- model/ - Exported RapidMiner Naive Bayes model
- data/ - Dataset description and source details
- app/ - Mendix application screenshots
- report/ - Project summary report (PDF)
- pitch/ - Presentation deck

---

## Impact
- Reduce unnecessary doctor visits for non-serious 
  conditions
- Early outbreak detection for 500+ villages through 
  anonymous symptom aggregation
- Save low-income families Rs 2,000-5,000 annually
- Scale from village to district to state level

---

## Roadmap
Phase 1 - Live: Symptom triage, doctor discovery, 
color coded risk levels
Phase 2 - Next 3 months: Live GPS location, live 
RapidMiner API endpoint, pre-visit intelligence
Phase 3 - 6-12 months: Voice input in Hindi, 
Marathi, and Pahari, health timeline, offline 
mode for 2G areas

---

Built for Bharat. Powered by AI.
Supported by RapidMiner + Mendix.# Aarogya AI
### India's first two-sided health intelligence 
platform - built for the last mile

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
500 million Indians lack access to affordable 
healthcare. The average doctor consultation fee of 
Rs 300-800 acts as a barrier for daily wage earners. 
58% of our survey respondents confirmed cost directly 
affects their doctor visit decisions. Minor illnesses 
become emergencies because people delay diagnosis.

---

## Solution
Aarogya AI serves two users simultaneously:

**For Patients:**
- Select symptoms via structured interface
- AI predicts disease with 99.3% accuracy
- Dynamic risk triage: Red (see doctor today) / 
  Yellow (monitor 3 days) / Green (home care)
- Nearest specialists shown with distance, 
  consultation fee, and rating
- Medical disclaimer on all results

**For Health Workers:**
- ASHA worker dashboard shows community symptom trends
- Anonymous aggregation detects disease outbreaks early
- Village-level alerts before outbreaks spread

---

## App Features
- 60 disease-symptom mappings including mental 
  health conditions
- Color coded risk levels (Red/Yellow/Green)
- Emergency escalation - critical symptoms like 
  chest pain immediately flag HIGH risk
- 3 nearest specialists with distance and 
  consultation fee
- REST API endpoint for live predictions
- Geoapify Places API integrated for real-time 
  doctor discovery (Phase 2 - live GPS location)

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

Note: 99.3% accuracy reflects performance on a 
clean structured Kaggle dataset. Real-world 
performance with noisy input will be validated 
in Phase 2 field testing.

---

## Tech Stack
| Tool | Purpose |
|---|---|
| Altair RapidMiner AI Studio | Data preprocessing, feature engineering, predictive modeling |
| Mendix Studio Pro | Patient app, ASHA dashboard, health map |
| Geoapify Places API | Real-time doctor and clinic discovery |

---

## Datasets
| Dataset | Source | Details |
|---|---|---|
| Disease Symptom Prediction | Pranay Patil, Kaggle | 4,920 examples, 41 diseases, 132 symptoms, 61,134 downloads |
| Doctor Specialty Recommendation | Ebrahim Elgazar, Kaggle | Maps diseases to correct specialist type |

---

## How It Works
1. Patient selects symptoms in Mendix app
2. Symptoms matched against RapidMiner Naive Bayes 
   model outputs stored in prediction table
3. Predicted disease, risk level, and specialist 
   recommendation returned in real time
4. Nearest specialists shown with distance, fee, 
   and rating
5. Anonymous symptom data aggregated for ASHA 
   worker outbreak alerts

Integration note: Current prototype uses 
RapidMiner-derived prediction table within Mendix 
for real-time matching. Phase 2 implements live 
REST API endpoint between Mendix and deployed 
RapidMiner model.

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
| Rated AI triage as highly useful | 47% |

---

## Repository Structure
aarogya-ai/
- README.md
- model/ - Exported RapidMiner Naive Bayes model
- data/ - Dataset description and source details
- app/ - Mendix application screenshots
- report/ - Project summary report (PDF)
- pitch/ - Presentation deck

---

## Impact
- Reduce unnecessary doctor visits for non-serious 
  conditions
- Early outbreak detection for 500+ villages through 
  anonymous symptom aggregation
- Save low-income families Rs 2,000-5,000 annually
- Scale from village to district to state level

---

## Roadmap
Phase 1 - Live: Symptom triage, doctor discovery, 
color coded risk levels
Phase 2 - Next 3 months: Live GPS location, live 
RapidMiner API endpoint, pre-visit intelligence
Phase 3 - 6-12 months: Voice input in Hindi, 
Marathi, and Pahari, health timeline, offline 
mode for 2G areas

---

Built for Bharat. Powered by AI.
Supported by RapidMiner + Mendix.# Aarogya AI
### India's first two-sided health intelligence 
platform - built for the last mile

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
500 million Indians lack access to affordable 
healthcare. The average doctor consultation fee of 
Rs 300-800 acts as a barrier for daily wage earners. 
58% of our survey respondents confirmed cost directly 
affects their doctor visit decisions. Minor illnesses 
become emergencies because people delay diagnosis.

---

## Solution
Aarogya AI serves two users simultaneously:

**For Patients:**
- Select symptoms via structured interface
- AI predicts disease with 99.3% accuracy
- Dynamic risk triage: Red (see doctor today) / 
  Yellow (monitor 3 days) / Green (home care)
- Nearest specialists shown with distance, 
  consultation fee, and rating
- Medical disclaimer on all results

**For Health Workers:**
- ASHA worker dashboard shows community symptom trends
- Anonymous aggregation detects disease outbreaks early
- Village-level alerts before outbreaks spread

---

## App Features
- 60 disease-symptom mappings including mental 
  health conditions
- Color coded risk levels (Red/Yellow/Green)
- Emergency escalation - critical symptoms like 
  chest pain immediately flag HIGH risk
- 3 nearest specialists with distance and 
  consultation fee
- REST API endpoint for live predictions
- Geoapify Places API integrated for real-time 
  doctor discovery (Phase 2 - live GPS location)

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

Note: 99.3% accuracy reflects performance on a 
clean structured Kaggle dataset. Real-world 
performance with noisy input will be validated 
in Phase 2 field testing.

---

## Tech Stack
| Tool | Purpose |
|---|---|
| Altair RapidMiner AI Studio | Data preprocessing, feature engineering, predictive modeling |
| Mendix Studio Pro | Patient app, ASHA dashboard, health map |
| Geoapify Places API | Real-time doctor and clinic discovery |

---

## Datasets
| Dataset | Source | Details |
|---|---|---|
| Disease Symptom Prediction | Pranay Patil, Kaggle | 4,920 examples, 41 diseases, 132 symptoms, 61,134 downloads |
| Doctor Specialty Recommendation | Ebrahim Elgazar, Kaggle | Maps diseases to correct specialist type |

---

## How It Works
1. Patient selects symptoms in Mendix app
2. Symptoms matched against RapidMiner Naive Bayes 
   model outputs stored in prediction table
3. Predicted disease, risk level, and specialist 
   recommendation returned in real time
4. Nearest specialists shown with distance, fee, 
   and rating
5. Anonymous symptom data aggregated for ASHA 
   worker outbreak alerts

Integration note: Current prototype uses 
RapidMiner-derived prediction table within Mendix 
for real-time matching. Phase 2 implements live 
REST API endpoint between Mendix and deployed 
RapidMiner model.

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
| Rated AI triage as highly useful | 47% |

---

## Repository Structure
aarogya-ai/
- README.md
- model/ - Exported RapidMiner Naive Bayes model
- data/ - Dataset description and source details
- app/ - Mendix application screenshots
- report/ - Project summary report (PDF)
- pitch/ - Presentation deck

---

## Impact
- Reduce unnecessary doctor visits for non-serious 
  conditions
- Early outbreak detection for 500+ villages through 
  anonymous symptom aggregation
- Save low-income families Rs 2,000-5,000 annually
- Scale from village to district to state level

---

## Roadmap
Phase 1 - Live: Symptom triage, doctor discovery, 
color coded risk levels
Phase 2 - Next 3 months: Live GPS location, live 
RapidMiner API endpoint, pre-visit intelligence
Phase 3 - 6-12 months: Voice input in Hindi, 
Marathi, and Pahari, health timeline, offline 
mode for 2G areas

---

Built for Bharat. Powered by AI.
Supported by RapidMiner + Mendix.
