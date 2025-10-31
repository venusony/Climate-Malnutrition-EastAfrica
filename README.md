# Climate-Malnutrition-EastAfrica
Data analysis and visualization project studying how climate variability (rainfall and temperature) affects child malnutrition trends in East Africa (2010–2024).

# Climate and Malnutrition in East Africa

This project explores how climate factors such as temperature and rainfall relate to child malnutrition trends in East Africa using Demographic and Health Survey (DHS) data from 2010 to 2024.

The analysis combines DHS child and maternal health indicators with CRU climate data to understand possible links between environmental changes and nutrition outcomes.

---

## Project Structure


---

## Research Goal

The main goal is to combine DHS data with CRU climate data to study how climate variability influences child nutrition outcomes such as stunting, wasting, and underweight prevalence.

Key questions:
- Does rainfall or temperature influence child height-for-age or weight-for-age?
- Are there observable malnutrition patterns by year or region?
- How do different countries compare across the 2010–2024 period?

---

## Project Phases

### Phase 1 — DHS Setup
- Download and unzip DHS ZIP files  
- Rename datasets by country and year  
- Review the DHS Recode Manual to understand variable codes  

### Phase 2 — Cleaning and Standardization
- Rename variable codes to descriptive names  
- Fix year and unit scales (children vs mothers)  
- Save final versions as Parquet and CSV files  

### Phase 3 — Stacking and Filtering
- Combine all survey years for each country  
- Filter datasets for 2010–2024  
- Create one merged dataset per country  

### Phase 4 — Climate Integration
- Load CRU temperature and rainfall data  
- Match DHS clusters using latitude and longitude  
- Merge climate and health datasets  

### Phase 5 — Analysis
- Calculate malnutrition indicators  
- Analyze trends and relationships with climate factors  
- Create plots and summaries by year and country  

---

## Tools Used
- Python (pandas, geopandas, matplotlib, seaborn)  
- Jupyter Notebook  
- GitHub for version control and project tracking  
- Excel for data inspection  

---

## Current Progress
- Cleaned and standardized DHS datasets for Ethiopia, Kenya, Uganda, and Tanzania  
- Renamed variables based on the DHS Recode Manual  
- Created Parquet and CSV versions for review  
- Next step: stack by country and prepare for CRU merge  

---

## Notes
- Double-check scaling for height and weight variables to avoid mixing child and maternal data  
- Keep separate columns for mother and child indicators  
- Use the official DHS Recode Manual in `/docs` for variable definitions  

---

## References
- Demographic and Health Surveys (DHS) Program: https://dhsprogram.com/  
- CRU Climate Data: https://crudata.uea.ac.uk/cru/data/hrg/  
- DHS Recode Manual (Phase VII, 2018) – included in `/docs/`

---


