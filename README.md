# U.S.-Severe-Weather-Event-Data-Visualization

*Course: IST 719 - Information Visualization - Syracuse University*

## Project Overview  
This mini-poster project analyzes decades of U.S. storm event data to uncover trends in storm frequency, severity, and human and economic impacts.  
The dataset—spanning 1958 to 2018, reveals clear patterns in storm activity, with notable increases beginning in the 1990s and peaking in the early 2010s before showing a gradual decline. While thunderstorm winds, hail, and flash floods are the most common event types, tornadoes consistently cause the highest death tolls, and hurricanes and floods generate the largest financial losses.

The final deliverable was an 8.5x11" or 11x17" PDF poster, synthesizing temporal, geographic, and impact-based visualizations into a cohesive narrative.

This project was completed in R, with final poster design and layout executed using standard data visualization and design tools.

---

## Dataset Description  

### **Source**
Data originates from the **NOAA National Weather Service Storm Events Database**.

### **Scope of Data**
- **Time range:** 1958–2018  
- **Geographic coverage:** All 50 U.S. states  
- **Storm types:** More than 40 event categories, including  
  - Thunderstorm wind  
  - Flash flood  
  - Hail  
  - Tornado  
  - Flood  
  - Lightning  
  - Marine hazards  
  - Rare events such as dust devils and debris flows  
- **Variables:**  
  - Event type  
  - Event year  
  - Fatalities and injuries  
  - Property and crop damage  
  - Geographic location (state / region)  

### **Key Metrics Extracted**
- Monthly and annual storm frequency  
- Top storm event categories  
- Geographic concentration of events  
- Economic damages (property + crop loss)  
- Casualties (fatal + non-fatal)  

---

## Methodology  

### Data Import & Cleaning
- Imported NOAA storm data using `readr`, `dplyr`, and `tidyverse` tools  
- Cleaned and standardized event types (removing duplicates / inconsistent labels)  
- Converted character fields for damages into numeric values  
- Aggregated events by year, state, and storm category  
- Validated missing data and ensured consistent temporal coverage  

### Data Transformation & Aggregation
To build the poster narrative, the dataset was transformed into multiple analytical tables:

- **Storm frequency by year**  
  - Summed total storm events annually  
  - Identified peak years (e.g., 2011 with 18,438 storms)

- **Top storm categories**  
  - Calculated percent contribution of each storm type  
  - Top 10 categories represented 92% of all 152,953 events

- **Regional event patterns**  
  - Mapped storm frequency by state  
  - Identified highest-activity states (e.g., Texas, Iowa, Ohio)

- **Damage metrics**  
  - Ranked storm types by  
    - Property damage  
    - Crop damage  
    - Total economic loss  
  - Extracted impact comparisons (e.g., floods wiping out $3.5B in crops)

- **Casualty analysis**  
  - Combined fatalities + injuries  
  - Identified tornadoes as highest-casualty storms
---

## Visualizations Featured in Poster  
The final poster included several coordinated graphics:

### **Monthly Storm Frequency (1958–2018)**
A 60-year time series showing rising storm event counts through the 1990s and 2000s, peaking in 2011.

### **U.S. Storm Event Density Map**
Choropleth map highlighting the geographic distribution of storm events.  
Highest concentrations:  
- **Texas (~9,500 events)**  
- **Iowa (~9,000)**  
- **Ohio (~7,800)**  

### **Most Common Storm Types (Top 10)**
Bar Chart breaksdown the major storm types and their share of total U.S. events:
- Thunderstorm Wind – **62%**  
- Flash Flood – **11%**  
- Hail – **8%**  
- Tornado – **7%**  
- Flood – **6%**  
- Lightning – **4%**  
- etc.

### **Top 5 Storm Event Metrics**
Radar chart comparing event types across:
- Frequency  
- Injuries  
- Crop damage  
- Property damage  
- Fatalities  

### **Asset Damage Metrics**
Callouts:
- Floods - $3.5B+ in crop loss  
- Flash floods - caused more property damage than any other storm type

### **Storm Casualties (Fatal + Non-Fatal)**
Bar chart shows Tornadoes leading casualties, followed by thunderstorm wind and floods.

---

## Key Insights  

- **Storm frequency has risen dramatically** since the 1990s.  
- **Thunderstorm winds dominate** event counts but are not always the deadliest or most damaging.  
- **Tornadoes cause the most casualties**, despite accounting for a smaller share of total storms.  
- **Floods and hurricanes drive the largest financial losses**, especially agricultural impacts.  
- **Storm activity clusters heavily in the South and Midwest**, particularly Texas, Iowa, and Ohio.  
- Peak activity around the early 2010s aligns with broader changes in climate patterns and reporting practices.  

---

## Tools

### **Visualization & Poster Design**
Visualizations were created in R, using packages such as:

- **ggplot2** – line plots, bar charts  
- **dplyr / tidyr** – data manipulation  
- **usmap / sf** – geographic mapping  
- **scales / RColorBrewer** – color palettes and formatting  

Color harmonization and annotation were completed in Adobe Illustrator to produce a clean, cohesive mini-poster.

---

## Poster

