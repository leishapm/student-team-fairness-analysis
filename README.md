# SC1003 Mini Project — Team Formation Fairness Analysis

## Done by
- Harry Choo Jin Rui (HCHOO004@e.ntu.edu.sg)
- Leisha Pritika Menezes (LEISHAPR001@e.ntu.edu.sg)
- Lee Xin Yin (XLEE067@e.ntu.edu.sg)
- Loh Kai Jun (KLOH014@e.ntu.edu.sg)
- Joshua Ling Soon Wah (JLING@e.ntu.edu.sg)

In fulfilment of the SC1003 Mini Project.

---

## Introduction

This project explores fairness in forming student teams for the "Introduction to Data Science" course.  
The cohort consisted of 6000 students divided into 120 tutorial groups of 50 each.  
The objective was to automatically form teams of five while ensuring fairness in terms of:

- School affiliation  
- Gender  
- CGPA  

The aim was to minimise clustering and create diverse, balanced teams across these attributes.

---

## Methodology

### Data Preparation
- Cleaned student data  
- Standardised categorical fields  
- Encoded gender, school, and CGPA information  

### Team Formation Approach
We compared several approaches, including random assignment and rule-based grouping.  
The final method grouped students into teams of five by minimising a fairness cost function that accounts for:
- CGPA variance  
- Gender balance  
- School diversity  

### Fairness Evaluation
We used:
- CGPA variance per team  
- Diversity metrics for school representation  
- Gender proportion balance  
- Aggregate fairness score combining all factors  

---

## Results

The final grouping achieved significantly improved fairness compared to random assignment.  
Teams showed:
- Lower CGPA disparity  
- More even distribution of schools  
- Balanced gender representation  

Detailed graphs and numerical results are included in the notebook.

---

## How to Run

### 1. Install Requirements
pip install -r requirements.txt

### 2. Open the Notebook
FDAD_Team3_LeishaMenezes.ipynb

### 3. Run All Cells  
This will:
- Load the dataset  
- Process the data  
- Form the teams  
- Compute fairness metrics  
- Generate analysis outputs  

---

## Files Included
- `FDAD_Team3_LeishaMenezes.ipynb` – full analysis and team formation workflow  
- `requirements.txt` – necessary packages  
- `records.csv` – dataset used for the project
- `LICENSE` – MIT License  

---

## Acknowledgements
We thank the SC1003 teaching team for providing the dataset and guidance.




