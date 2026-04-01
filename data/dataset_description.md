# Dataset Description

## Primary Dataset

**Name:** Disease Symptom Prediction  
**Author:** Pranay Patil  
**Source:** Kaggle (61,134 downloads — widely validated across research papers)  
**License:** Public Domain  

### Structure
| Property | Value |
|---|---|
| Total records | 4,920 |
| Disease classes | 41 |
| Symptom features | 132 |
| Examples per class | 120 (perfectly balanced) |
| Class imbalance | None |
| Missing values | None |

### Feature Engineering
Each of the 132 symptoms is encoded as a binary presence/absence feature:
- Value of `1` indicates the symptom was reported by the patient
- Value of `0` indicates the symptom was absent
- No normalization required as all features share the same binary scale
- The full 132-feature space was preserved to distinguish clinically 
  similar diseases such as Dengue and Malaria

### Disease Classes (41 total)
Includes but not limited to:
- Dengue Fever, Malaria, Typhoid (infectious/vector-borne)
- Diabetes, Hypertension (chronic conditions)
- Fungal Infection, Allergy (dermatological/immunological)
- Bronchial Asthma, Tuberculosis (respiratory)
- GERD, Peptic Ulcer, Jaundice (gastrointestinal/hepatic)
- Cervical Spondylosis, Arthritis (musculoskeletal)

### Why This Dataset Was Selected
- Perfectly balanced classes eliminate model bias toward frequent diseases
- 132 symptom features provide sufficient granularity for Naive Bayes 
  conditional probability estimation
- 61,134 Kaggle downloads confirm community validation
- Consistent with symptom patterns observed in Indian primary care settings

### Validation Performance on This Dataset
- Algorithm: Naive Bayes (best of 205 Auto Model configurations)
- Accuracy: 99.3%
- Classification Error: 0.7%
- Standard Deviation: +/- 0.4% (multiple hold-out cross-validation)

### Confusion Matrix Highlights
| Disease | Correct | Total | Accuracy |
|---|---|---|---|
| Allergy | 38 | 38 | 100% |
| Diabetes | 36 | 36 | 100% |
| Dengue Fever | 35 | 35 | 100% |
| GERD | 30 | 30 | 100% |
| Fungal Infection | 32 | 34 | 94% |

---

## Secondary Dataset

**Name:** Doctor Specialty Recommendation  
**Author:** Ebrahim Elgazar  
**Source:** Kaggle  
**Purpose:** Maps predicted diseases to correct doctor specialization

### Structure
| Property | Value |
|---|---|
| Function | Disease to specialist mapping |
| Usage | Post-prediction routing |
| Integration | Lookup against predicted disease output |

### Specialist Mappings (examples)
| Predicted Disease | Specialist Type |
|---|---|
| Dengue Fever | Infectious Disease |
| Fungal Infection | Dermatologist |
| Allergy | ENT Specialist |
| Bronchial Asthma | Pulmonologist |
| GERD | Gastroenterologist |
| Malaria | Infectious Disease |
| Typhoid | General Physician |
| Tuberculosis | Pulmonologist |
| Diabetes | Endocrinologist |
| Jaundice | Gastroenterologist |

---

## Integration Architecture

```
Patient Symptoms (input)
        |
        v
Symptom-Disease Mapping Table (Mendix)
        |
        v
Predicted Disease + Risk Level + Recommended Action
        |
        v
Specialist Type (from secondary dataset mapping)
        |
        v
Nearest Doctors by Specialty (output)
```

Phase 2 will replace the mapping table with a live REST API 
endpoint connected to a deployed RapidMiner Naive Bayes model 
for fully dynamic inference.

---

## Data Ethics
- No personally identifiable information (PII) in either dataset
- Both datasets are publicly available on Kaggle
- Disease prediction is for triage guidance only, not medical diagnosis
- All outputs include disclaimer to consult a qualified medical professional
