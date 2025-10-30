#  Aviation Risk Analysis Project

## Overview
This project analyzes aviation accident and incident data to identify the safest aircraft types and flight conditions for a new aviation business.  
By exploring historical safety records, the goal is to support evidence-based decision-making for fleet selection, pilot training priorities, and operational safety strategies.

The analysis was conducted in Python using **Pandas**, **NumPy**, and **Matplotlib** within a Jupyter Notebook.  
Both the notebook (`Aviation_analysis.ipynb`) and a final report in PDF format are available in this repository.

---

## Business Understanding

### Stakeholders
- **Aviation management team** — evaluating aircraft safety before fleet acquisition.  


### Key Business Questions
1. Which aircraft manufacturers and models demonstrate the strongest safety records?  
2. During which phases of flight do most injuries occur, and how can risks be mitigated?  
3. How have aviation safety outcomes evolved over time?

By addressing these questions, the company can make data-driven decisions that enhance operational safety and reduce financial risk.

---

## Data Understanding and Analysis

### Source of Data
The dataset was sourced from [Kaggle – Aviation Accidents and Incidents (NTSB, FAA, WAAS)](https://www.kaggle.com/datasets/prathamsharma123/aviation-accidents-and-incidents-ntsb-faa-waas?resource=download&select=airline_accidents.csv).  
It contains over **90,000 records** of aviation accidents and incidents, including details such as:
- Aircraft make and model  
- Date and location of event  
- Phase of flight  
- Injury severity (fatal, serious, minor, uninjured)

### Description of Data
After cleaning and preparation:
- **Rows:** 87,951 → reduced  after removing duplicates and missing records  
- **Columns used:** `Make`, `Model`, `Event_Date`, `Purpose_of_flight`, `Broad_phase_of_flight`, `Total_Fatal_Injuries`, `Total_Serious_Injuries`, `Total_Minor_Injuries`, `Total_Uninjured`  
- **Missing values:** Imputed with median for numeric columns; categorical columns were standardized and filled with `"Missing"` or `"Unknown"` as appropriate.

### Key Visualizations

#### 1. Top 10 Aircraft Makes by Total Uninjured Passengers
Boeing aircraft recorded the highest number of uninjured passengers, suggesting strong safety performance.

![Top 10 Aircraft Makes by Total Uninjured]('./images/Top_10_Makes_by_Uninjured.png')

#### 2. Total Injuries by Phase of Flight
Takeoff, cruise, and maneuvering phases had the highest number of injuries, highlighting critical safety periods.

![Total Injuries by Phase of Flight]('./images/Total_injuries_by_phase_of_flight.png')

#### 3. Trend of Total Injuries Over Time
Injuries have steadily declined since the 1980s, reflecting advancements in aviation technology and safety regulation.

![Trend of Injuries Over Time]('./images/Trend_of_total_injuries_over_time.png')

*(Each visualization was created in the notebook and exported to the `images/` folder for reference.)*

---

## Conclusion

### Summary of Findings
1. **Boeing aircraft** showed the best safety performance based on uninjured passenger counts.  
2. **Takeoff and cruise phases** are the most accident-prone stages of flight.  
3. **A steady decline in injuries** over the past decades demonstrates significant improvement in aviation safety standards.

### Recommendations
- **Fleet Selection:** Prioritize aircraft from manufacturers with strong historical safety records (e.g., Boeing).  
- **Training Focus:** Emphasize pilot proficiency in takeoff, cruise, and maneuvering phases.  
- **Continuous Monitoring:** Maintain data-driven safety audits to ensure long-term operational safety improvements.

---



---

**Author:** Grace Wangui

 
**Tools:** Python, Pandas, Matplotlib, NumPy, Jupyter Notebook  
**License:** MIT 
````




