
# Air Pollution Analysis with R 🌍

## Overview  
This project analyzes air pollution data in India 🇮🇳 using R 🧑‍💻. It focuses on understanding pollution trends by state and year 📅 and visualizing metrics such as SO2, NO2, RSPM, SPM, and EMIS content across various regions 🌆.  

## Table of Contents  
1. [Setup and Requirements](#setup-and-requirements) 🛠️  
2. [Data Preprocessing](#data-preprocessing) 🔧  
3. [Visualization and Analysis](#visualization-and-analysis) 📊  
4. [Key Visualizations](#key-visualizations) 🎨  
5. [Conclusion](#conclusion) 📍  

---

### Setup and Requirements 🛠️  

#### R Libraries 📦  
Ensure you have the following libraries installed before running the script:  
```R  
install.packages("high")  
library(ggplot2)  
library(dplyr)  
library(tidyr)  
library(highcharter)  
library(lubridate)  
library(xts)  
library(reshape2)  
```  

#### Data File 📄  
The script expects a CSV file named `data.csv` with columns:  
- `date`  
- `state`  
- `type`  
- `so2`, `no2`, `rspm`, `spm`, `emis`  

Place the file in your working directory. 📂  

---

### Data Preprocessing 🔧  
1. **Date Formatting** 🗓️: The `date` column is converted to `Date` and `POSIXct` formats.  
2. **Category Cleanup** 🧹: `type` categories are consolidated into broader groups:  
   - "Sensitive Areas" → "Sensitive Area"  
   - "Industrial" & "Industrial Areas" → "Industrial Area"  
   - "Residential" → "Residential and others"  

---

### Visualization and Analysis 📊  

#### State-wise Averages 📉  
Grouped by state, average levels of SO2, NO2, RSPM, SPM, and EMIS are calculated and visualized.  

#### Delhi Trends 📍  
Year-wise pollution trends for Delhi are analyzed using line plots with `facet_wrap` for pollution types.  

#### State-Year Longitudinal Data 📆  
Longitudinal data for all states is analyzed and visualized:  
- Heatmaps 🌡️  
- Bar charts 📊  

---

### Key Visualizations 🎨  

1. **State-wise Bar Charts 📊**:  
   - Average SO2, NO2, RSPM, SPM, and EMIS content.  
   - Highlight significant pollution levels by state.  

2. **Delhi Pollution Trends 📍**:  
   - Year-wise trends for SO2, NO2, RSPM, SPM, and EMIS.  
   - Faceted views by pollution type for detailed analysis.  

3. **Heatmaps 🌡️**:  
   - Visualize yearly pollution levels (SO2, NO2, RSPM, SPM, and EMIS) by state.  

---

### Conclusion 📍  

This project provides a comprehensive overview of air pollution trends in India, enabling stakeholders to identify problem areas and prioritize actions. The visualizations are key to communicating data insights effectively.  

For further information or contributions, feel free to submit issues or pull requests. 🤝

---
