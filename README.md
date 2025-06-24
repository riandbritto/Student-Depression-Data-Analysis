# Student-Depression-Data-Analysis
# README: Student Mental Health and Academic Performance Dashboard

## Overview
This Tableau dashboard analyzes the relationship between various student lifestyle factors (sleep, study habits, academic pressure, financial stress) and their academic performance/mental health. The data is sourced from an Azure database server.

## Dashboard Components

### 1. Sleep Duration Analysis
- **Categories**: 
  - 5-6 hours
  - 7-8 hours 
  - Less than 5 hours
  - More than 8 hours
- **Visualization**: Shows student count distribution across different sleep durations

### 2. Study Hours Analysis
- **Metrics**:
  - Student Count (SC) across different study hour ranges
- **Data Points**:
  - SC-13, SC-8, SC-6, SC-7, SC-4 (representing counts for different study hour brackets)

### 3. Study Satisfaction
- **Scale**: SS-1 to SS-5 (1 being lowest satisfaction)
- **Visualization**: Correlates satisfaction levels with student counts (SC-86 to SC-116)

### 4. Academic Pressure
- **Scale**: AP-1 to AP-5 (1 being lowest pressure)
- **Data Points**:
  - AP-2 SC-25
  - AP-3 SC-22
  - AP-4 SC-17
  - AP-1 SC-17
  - AP-5 SC-16

### 5. Financial Stress
- **Scale**: FS-1 to FS-5 (1 being lowest stress)
- **Data Points**:
  - FS-1 SC-25
  - FS-5 SC-23
  - FS-4 SC-19
  - FS-2 SC-18
  - FS-3 SC-12

## Data Structure
The underlying data model includes these key dimensions:
- Academic Pressure
- Age Group
- Depression indicators
- Dietary Habits
- Family History of Mental Illness
- Financial Stress
- Gender
- Suicidal ideation history
- Sleep Duration
- Study Hours
- Study Satisfaction

## Filters and Controls
The dashboard includes interactive filters for:
- Study Satisfaction levels
- Sleep duration categories
- Academic pressure levels
- Financial stress levels
- Study hour ranges

## Data Source
- **Connection**: Azure Database Server
- **Tables**: Multiple tables joined through Measure Values and Index Columns
- **Record Count**: Approximately 97-502 records depending on the view

## How to Use
1. Select different filter options to explore relationships between factors
2. Hover over data points to see detailed student counts
3. Compare different metrics using the various sheets in the dashboard
4. Use the "Show Me" feature to change visualization types

## Insights Potential
This dashboard can help identify:
- Optimal sleep durations for student performance
- Correlation between academic pressure and mental health
- Impact of financial stress on study habits
- Relationship between study hours and satisfaction levels

## Technical Notes
- Dashboard uses calculated fields like "Depression+Student+Data"
- Some measures are aggregated using SUM of CNT functions
- Data is scaled to show relative proportions between categories
