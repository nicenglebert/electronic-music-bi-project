# Electronic Music Business Intelligence Project 🎧📊

![Power BI](https://img.shields.io/badge/Tool-Power%20BI-yellow)
![ETL](https://img.shields.io/badge/Process-ETL-blue)
![Data Warehouse](https://img.shields.io/badge/Model-Star%20Schema-green)
![Status](https://img.shields.io/badge/Status-Completed-success)


A complete **Business Intelligence project** analyzing electronic music trends using Spotify data and European festival datasets.  
This project demonstrates a full **data pipeline** from raw CSV data to interactive dashboards using Power BI and dimensional modeling.

---

## 🚀 Project Overview

This project explores electronic music through two complementary perspectives:

- 🎵 **Music production & popularity** (Spotify dataset)
- 🎪 **Festivals & events analytics** (Festival Alarm scraping)

The goal is to demonstrate:
- Data transformation using Power Query
- Data warehouse design (star schema)
- KPI calculations (DAX)
- Interactive dashboards
- Analytical storytelling

---

## 🧱 Architecture & Data Pipeline

SOURCE (CSV / Scraping)
↓ Extract
STAGING AREA (Power Query cleaning)
↓ Transform
DATA WAREHOUSE (Star Schema)
↓ Load & Connect
POWER BI DASHBOARDS


🧠 This project follows a classical BI architecture:
- Extract → Transform → Load
- Staging layer for cleaning & normalization
- Dimensional model (facts & dimensions)
- Analytical dashboards powered by DAX measures

📐 Architecture diagram available here:  
<img width="504" height="520" alt="image" src="https://github.com/user-attachments/assets/bcaf7674-675d-434f-8caf-7e0f5190dfc1" />


---

## 📁 Repository Structure

```text
electronic-music-bi-project/
│
├── dashboards/
│   └── powerbi/
│       └── Projet_Techno_Nicolas_Englebert.pbix
│
├── data/
│   ├── raw/              # Original CSV sources (Kaggle + Scraping)
│   ├── staging/          # Cleaned datasets (Power Query export)
│   └── model/            # Star schema tables (Facts & Dimensions)
│
├── docs/
│   ├── Executive_Summary_Project_BI.pdf
│   └── Projet BI Musiques électroniques & Festivals.pptx
│
├── screenshots/
│   ├── Executive_Summary.PNG
│   ├── Festivals KPI Dashboard.PNG
│   ├── Spotify KPI Dashboard.PNG
│   ├── model_view.PNG
│   └── BI_Architecture.PNG
│
├── README.md
├── Methodology.md
└── BI_Architecture.PNG



---

## 📊 Key Dashboards

### Spotify Analytics
- Popularity by genre
- BPM distribution
- Track volume by year
- Average duration
- Genre dominance

### Festival Analytics
- Total festivals by country
- Visitors per genre
- Monthly seasonality
- Ticket price analysis
- Genre segmentation

## 📊 Dashboards Preview

### Executive Summary
![Executive Summary](screenshots/Executive_Summary.PNG)

### Festivals Analytics
![Festivals Dashboard](screenshots/Festivals_KPI_Dashboard.PNG)

### Spotify Analytics
![Spotify Dashboard](screenshots/Spotify_KPI_Dashboard.PNG)


## Key Insights

### 🎧 Spotify Trends
- House and Deep House are the most represented genres in the dataset.
- The average BPM is around **127**, consistent with techno/house norms.
- Most tracks are between **3 and 5 minutes**, with techno tracks being longer on average.
- Popularity differs significantly by genre, with melodic genres performing better.

### 🎪 Festival Analytics
- Electronic festivals are mainly concentrated between **June and August**.
- Average ticket price is approximately **€97**.
- Germany, France, and UK host the highest number of festivals.
- The most common genres are **Electro, House, and Techno**.
- Average attendance per festival is around **32,000 people**.

### 🔗 Cross-domain Observations
- High-popularity genres on Spotify are also the most represented at festivals.
- BPM averages are consistent between recorded music and live performances.
- Electronic music shows strong seasonal and geographic concentration in Europe.



---

## 📈 Key Insights

- 🎧 Most dominant genres: **House, Tech House & Electro**
- ⚡ Average BPM ≈ **127**
- ⏱ Average track duration ≈ **4 minutes**
- 🎟️ Ticket prices ≈ **€98 average**
- 👥 Attendance ≈ **32k visitors per festival**
- ☀️ Festivals have strong seasonality (summer peak)

---

## 🔧 Technologies Used

- Power BI Desktop
- Power Query (ETL)
- DAX
- CSV datasets
- GitHub for portfolio
- WebScraper.io
- Star schema modeling

---

## ▶️ How to Run the Project

1. Clone or download this repository
2. Open the `.pbix` file in Power BI
3. Refresh data connections (if needed)
4. Explore dashboards and filters

---

## 📜 Documentation

- Executive Summary (PDF)
- Presentation slides
- Methodology.md (ETL & design explanation)
- Star schema diagram

---

## 👤 Author

**Nicolas Englebert**  
Business Intelligence / Data Analytics  
📎 LinkedIn: https://www.linkedin.com/in/nicolas-englebert-2original  
📁 GitHub: https://github.com/nicenglebert

---

## ⚠️ Disclaimer

All datasets are used for **educational and portfolio purposes only**.  
Music data belongs to respective rights holders.

---

























