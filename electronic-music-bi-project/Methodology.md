# Methodology – BI Project Workflow

## 1. Business Goal

The main goal of this project is to analyze trends in electronic music using both:
- Spotify track-level data
- Electronic music festival data

The purpose is to identify:
✔ genre popularity  
✔ BPM trends  
✔ geographic distribution  
✔ pricing strategies  
✔ seasonality patterns  
✔ audience behaviors  

This project is designed as a full **Business Intelligence pipeline** rather than a simple data visualization exercise.

---

## 2. Data Sources

Two main sources were used:

### Spotify Dataset
- Extracted from Kaggle
- Format: CSV
- Contains: track name, artist, BPM, duration, genre, popularity, year

### Festival Dataset
- Web scraping using WebScraper.io
- Source website: festival-alarm.com
- Data collected: festival name, location, genre, price, visitors, dates

---

## 3. Data Pipeline Architecture

The BI pipeline follows a classical architecture:

SOURCE → ETL → STAGING → DATA WAREHOUSE → DASHBOARDS

---

## 4. ETL Process (Power Query)

All processing is done with Power Query:

### Extract
Import CSV files from:
- Kaggle exports
- WebScraper output

---

### Transform

Main transformations:
- Column standardization
- Text cleaning
- Genre normalization
- Date formatting
- KPI preparation (duration conversion, BPM filtering)
- Duplicate removal
- Referential integrity checks

---

### Load (Staging Layer)

Cleaned datasets are exported:
- One dataset per domain
- Structured as staging CSV files

Folder:
`/data/staging/`

Example:
- Spotify_cleaned.csv
- Festivals_cleaned.csv
- countries_cleaned.csv

---

## 5. Data Warehouse Design

A star schema was implemented:

### Fact tables
- FactTracks
- FactFestivalBase
- FactFestivalGenres

### Dimension tables
- DimArtistTracks
- DimGenreTracks
- DimGenresFestival
- DimTimeTracks
- DimTimeFestival
- DimCityFestival
- DimCountryFestival

This architecture ensures:
✅ better performance  
✅ analytical consistency  
✅ scalable design  

Diagram available in:
`screenshots/model_view.PNG`

---

## 6. Power BI Modeling

The Power BI data model integrates:
- Fact tables with proper relationships
- Time dimension for trend analysis
- Measures for KPIs:
  - Average BPM
  - Popularity score
  - Visitor average
  - Festival count
  - Price segmentation

---

## 7. Dashboard Design Principles

Key concepts:
- KPI orientation
- Visual hierarchy
- Clear segmentation by theme
- Interactivity via slicers
- Focus on insights, not charts

---

## 8. Final Objective

This project replicates a real-world BI workflow, from raw data to executive dashboards, demonstrating:

✔ data engineering logic  
✔ dimensional modeling  
✔ business insight delivery  
✔ dashboard storytelling  





