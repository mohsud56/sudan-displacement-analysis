# Sudan Conflict Displacement Analysis

![Project Banner](https://static.wixstatic.com/media/df1038_8d89ea6360e54e01b9785f62774a8a5e~mv2.png/v1/fill/w_1000,h_1000,al_c,q_90,usm_0.66_1.00_0.01/df1038_8d89ea6360e54e01b9785f62774a8a5e~mv2.png)  
*(Map by Béla Müller, Genocide Watch)*

## Overview
As a Sudanese who is passionate about humanitarian issues in Sudan, I built this project to highlight the displacement crisis using open data.

This is my data analysis project on the ongoing war in Sudan and how it's causing massive displacement and migration. I put this together using real numbers from sources like ACLED and UNHCR. The whole thing was built on my phone with Google Colab – no fancy setup, just me figuring it out step by step.

**What's This About?**
The civil war in Sudan kicked off in April 2023 between the SAF and RSF, and it's led to one of the biggest humanitarian crises right now. Over 11 million people have been forced from their homes – some staying inside Sudan as IDPs, others fleeing to neighboring countries. I wanted to dig into the data to see how violence (like fatalities from clashes) ties into this displacement mess.
Key stuff I found:

Total fatalities reported since April 2023: around 52,125 (pulled from ACLED data).
Total conflict events: about 14,581.
From UNHCR (as of early 2026): Roughly 7.1 million IDPs in Sudan, 3.5 million refugees who've left, totaling 11.8 million displaced folks.
Hardest-hit areas: Places like Khartoum, North Darfur, and Central Darfur have the most fatalities, which probably explains the migration waves from there.

I used Python in Colab for everything – cleaning data, running calculations, and making charts. It's my way of practicing data skills while shining a light on something important.

**Key Problem Addressed**: How has conflict intensity (measured by fatalities and events) driven one of the world's largest displacement crises, affecting over 11.8 million people?

**Key Findings**:
- Total fatalities since April 2023: ~52,125 (from ACLED data).
- Total events: ~14,581.
- UNHCR estimates: ~7.1M internally displaced persons (IDPs), ~3.5M refugees fled Sudan.
- Regions with highest fatalities: Khartoum, North Darfur, Central Darfur (see visuals below).

This project demonstrates skills in data cleaning, analysis, visualization, and GitHub deployment. Built entirely on a mobile device using Google Colab for accessibility.

## Tasks and Accomplishments
Here's a breakdown of the key tasks I completed in this project, Here's how I tackled the project step-by-step:
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
![Monthly Fatalities]<img width="784" height="525" alt="newplot-1" src="https://github.com/user-attachments/assets/6976bd94-4fa1-4a7d-977b-56c9fbbaf03c" />
*( peaks in 2023-2024 correlate with major displacement.)*

### Top Regions by Fatalities
![Regions Bar Chart]<img width="784" height="525" alt="newplot" src="https://github.com/user-attachments/assets/13e83347-3810-4911-9427-942bace22380" />  
*(Interactive: The bar chart effectively highlights the regions most affected by conflict fatalities in Sudan since April 2023.)*

## Future Improvements
- Add geospatial mapping (e.g., with Folium) for regional visuals.
- Integrate real-time UNHCR API for dynamic displacement data.
- Expand to predictive modeling (e.g., forecast displacement based on fatalities).

This project highlights my ability to handle real-world data problems, from sourcing to visualization, in a resource-constrained environment. Feel free to fork or contact me for collaborations!

**Author**: Mohammed Amin
**Date**: January 17, 2026  
**LinkedIn**: (https://www.linkedin.com/in/mohamed-amin-hussein/)
