# Sudan Conflict Displacement Analysis

![Project Banner](https://static.wixstatic.com/media/df1038_8d89ea6360e54e01b9785f62774a8a5e~mv2.png/v1/fill/w_1000,h_1000,al_c,q_90,usm_0.66_1.00_0.01/df1038_8d89ea6360e54e01b9785f62774a8a5e~mv2.png)  
*(Map by Béla Müller, Genocide Watch)*

## Overview
This repository contains a data analysis project examining the impact of the ongoing civil war in Sudan (starting April 2023) on displacement and migration. Using real data from ACLED (Armed Conflict Location & Event Data Project) and UNHCR, the project analyzes trends in political violence events, fatalities, and their correlation with displacement figures. The analysis is performed in Python via Google Colab, with interactive visualizations using Plotly.

**Key Problem Addressed**: How has conflict intensity (measured by fatalities and events) driven one of the world's largest displacement crises, affecting over 11.8 million people?

**Key Findings**:
- Total fatalities since April 2023: ~52,125 (from ACLED data).
- Total events: ~14,581.
- UNHCR estimates: ~7.1M internally displaced persons (IDPs), ~3.5M refugees fled Sudan.
- Regions with highest fatalities: Khartoum, North Darfur, Central Darfur (see visuals below).

This project demonstrates skills in data cleaning, analysis, visualization, and GitHub deployment. Built entirely on a mobile device using Google Colab for accessibility.

## Tasks and Accomplishments
Here's a breakdown of the key tasks I (Mohammed) completed in this project, showcasing my end-to-end data analysis workflow:

### 1. **Data Sourcing and Preparation**
   - Sourced real, aggregated monthly conflict data from ACLED (Excel file: `sudan_hrp_political_violence_events_and_fatalities_by_month-year_as-of-15jan2026.xlsx`).
   - Integrated static displacement statistics from UNHCR (latest as of Jan 2026).
   - Cleaned data: Converted month/year to datetime, filtered for April 2023–Jan 2026, handled regional aggregation (Admin1/Admin2).
   - Accomplishment: Handled large dataset (~68,000 rows) efficiently in Pandas, summing national and regional totals without errors.

### 2. **Analysis**
   - Calculated national totals: Fatalities, events since war start.
   - Grouped data monthly for trend analysis (e.g., peak fatalities in key months).
   - Regional breakdown: Summed fatalities by Admin1 (states like Khartoum, Darfur regions) to identify hotspots.
   - Linked conflict trends to displacement: Noted correlations between fatality spikes and migration waves.
   - Accomplishment: Used Pandas for grouping/aggregation; added custom date handling to ensure accurate time-series analysis.

### 3. **Visualizations and Dashboard**
   - Created interactive Plotly charts:
     - Line chart: Monthly fatalities (zoomable, shows trends like initial surge in 2023).
     - Bar chart: Monthly events vs. fatalities (grouped for comparison).
     - Bar chart: Top regions by fatalities (colored gradient, sorted descending).
   - Built a simple "dashboard" in the notebook for exploring trends.
   - Accomplishment: Ensured mobile-friendly visuals (rotated labels, adjustable height); fixed issues like axis scaling and indentation errors during development.

### 4. **Deployment to GitHub**
   - Created a new repository: `sudan-displacement-analysis`.
   - Saved Colab notebook directly to GitHub.
   - Uploaded data file and added this README.
   - Accomplishment: Managed entire process on a phone browser, demonstrating adaptability and beginner-level GitHub proficiency.

### Challenges Overcome
- Worked exclusively on mobile (no computer access).
- Debugged code issues (e.g., IndentationErrors, axis labeling) in real-time.
- Ensured compliance with ACLED terms of use (no raw data sharing, proper attribution).

## How to Run the Project
1. **Open the Notebook**: View `sudan_analysis.ipynb` in this repo (GitHub renders it with plots).
2. **Run in Colab**:
   - Click "Open in Colab" from GitHub.
   - Upload the Excel data file when prompted.
   - Run all cells to see analysis and interactive dashboards.
3. **Requirements**: No installation needed—uses Google Colab with Pandas, Plotly, and OpenPyXL.

## Data Sources and Attribution
- **ACLED**: Political violence data from [ACLED Sudan HRP Dataset](https://acleddata.com/data-export-tool/) (as of Jan 15, 2026). Used under [ACLED Terms of Use](https://acleddata.com/terms-of-use/).
- **UNHCR**: Displacement figures from [UNHCR Sudan Situation Portal](https://data.unhcr.org/en/situations/sudansituation) (latest: ~11.8M displaced).
- All data processed ethically; no raw distribution.

## Visual Examples
### Monthly Fatalities Trend
![Monthly Fatalities](https://via.placeholder.com/800x400?text=Sample+Line+Chart:+Monthly+Fatalities)  
*(Run the notebook for interactive version; peaks in 2023-2024 correlate with major displacement.)*

### Top Regions by Fatalities
![Regions Bar Chart](https://via.placeholder.com/800x400?text=Sample+Bar+Chart:+Fatalities+by+Region)  
*(Interactive: Hover for exact numbers; Khartoum often tops due to urban fighting.)*

## Future Improvements
- Add geospatial mapping (e.g., with Folium) for regional visuals.
- Integrate real-time UNHCR API for dynamic displacement data.
- Expand to predictive modeling (e.g., forecast displacement based on fatalities).

This project highlights my ability to handle real-world data problems, from sourcing to visualization, in a resource-constrained environment. Feel free to fork or contact me for collaborations!

**Author**: Mohammed Amin
**Date**: January 17, 2026  
**LinkedIn**: (https://www.linkedin.com/in/mohamed-amin-hussein/)
