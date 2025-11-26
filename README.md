# STAT172_Project1

# Predicting NCAA Tournament Selection with Logistic Regression

**Group:** Jaxon Hicks, Joseph Joswiak, Levi Sneller  
**Project Type:** Binary Classification / Generalized Linear Model (Logistic Regression)

---

## Project Overview

This project applies **logistic regression** to predict whether a Division I NCAA basketball team will make the NCAA Tournament based on season performance metrics and conference classification.

Using real NCAA basketball data, we estimate **odds ratios, confidence intervals, hypothesis tests, and probabilities** to answer sports analytics questions including:

- How do wins and offensive efficiency affect tournament selection?
- How much does conference strength matter?
- What offensive efficiency guarantees a 95% chance of making the tournament?

---

## Dataset

- **Source:** Kaggle – College Basketball Dataset  
- **File:** `cbb.csv`  
- **Observations:** NCAA Division I teams (season-level data)

### Variables

- Gi represent the number of games played by team i
- Wi represent the number of games won by team i
- ADJOEi represent team i’s adjusted offensive efficiency
- ADJDEi represent team i’s adjusted defensive efficiency
- BARTHAGi represent team i’s power rating (chance of beating an average D1 team)
- EFG_Oi represent team i’s effective field goal percentage shot
- EFG_Di represent team i’s effective field goal percentage allowed
- ADJ_Ti represent team i’s effective adjusted tempo
- LMi = 1 if team i is part of the LM conference group, and 0 otherwise
- MMi = 1 if team i is part of the MM conference group, and 0 otherwise

---

## Data Cleaning & Code (SAS)

All data preparation was completed in **SAS** using:

- Conversion of `POSTSEASON` into a **binary Bernoulli variable**
- Conference classification into:
  - **Power 5 (P5)**
  - **Mid-Major (MM)**
  - **Low-Major (LM)**
- Removal of excessive categorical levels
- Frequency tables used to validate transformations

