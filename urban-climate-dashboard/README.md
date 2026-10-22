# 🌆 Urban Climate Dashboard

An interactive web dashboard visualizing climate data for **20 major cities** across **4 continents** spanning **45 years (1980–2025)**.

[![Open Dashboard](https://img.shields.io/badge/Open-Dashboard-blue?style=for-the-badge)](./index.html)

---

## 🔴 Live Preview

Just download and open `index.html` in any browser — **no internet or server needed**.

---

## 📊 Features

| Chart | Description |
|---|---|
| 📈 Annual Trend | Year-by-year metric trend for selected city (1980–2025) |
| 📅 Monthly Profile | Month-by-month breakdown for selected city & year |
| 📊 City Comparison | Bar chart ranking all cities by selected metric |
| 🍩 Continent Donut | Proportional continent share of selected metric |
| 🔵 Scatter Plot | Temperature vs Humidity for all cities |
| 🃏 Stat Cards | Live snapshot of all 5 metrics for selected city & year |

---

## 🎛️ Interactive Controls

- **City** — Select from 20 global cities
- **Metric** — Temperature · Humidity · Precipitation · Wind Speed · Urban Heat Island
- **Continent Filter** — Americas · Asia · Europe · Africa
- **Year Slider** — Scrub any year from 1980 to 2025

---

## 📁 Project Structure

```
urban-climate-dashboard/
│
├── index.html                  ← Main dashboard (open this in browser)
│
├── data/
│   └── urban_climate_cleaned.csv   ← Source dataset (11,040 rows)
│
├── scripts/
│   ├── build_dashboard.py      ← Python script that generated index.html
│   └── gen_charts.py           ← Python script that generated chart images
│
├── charts/
│   ├── chart1.png              ← Annual Trend chart
│   ├── chart2.png              ← Monthly Profile chart
│   ├── chart3.png              ← City Comparison bar chart
│   ├── chart4.png              ← Continent Donut chart
│   └── chart5.png              ← Scatter Plot
│
├── report/
│   └── Urban_Climate_Dashboard_Report.docx  ← Full project report
│
└── README.md
```

---

## 🔑 Key Insights

- 🌡️ **Global temperatures rose +0.93°C** from 1980 to 2025 (climate change evidence)
- 🥵 **Lagos is the hottest city** — 35.15°C average across all years
- 🥶 **Berlin is the coldest** — -1.59°C average
- 🌧️ **Mumbai & Lagos get the most rainfall** — ~81 mm/month avg
- 🏙️ **Urban Heat Island** intensity of 2.0 in New York, Tokyo, Delhi, Beijing
- 🌍 **Africa vs Europe** — a 35°C temperature gap between continents

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| Python (`csv`, `json`) | Data processing & aggregation |
| HTML5 + CSS3 | Page structure & styling |
| JavaScript (Vanilla) | Filtering, events, rendering |
| HTML5 Canvas API | Drawing all charts from scratch |
| Tailwind CSS | Layout utilities |
| Matplotlib | Generating chart images for report |

> **No external charting libraries used** (no Chart.js, D3.js, or Plotly).

---

## 📦 Dataset

- **File:** `urban_climate_cleaned.csv`
- **Cities:** 20 major global cities
- **Period:** 1980 – 2025 (monthly)
- **Records:** 11,040 rows
- **Metrics:** Temperature, Humidity, Precipitation, Wind Speed, Urban Heat Island Intensity

---

## 🚀 How to Run

```bash
# Option 1 — Just open in browser (no setup needed)
open index.html

# Option 2 — Rebuild the dashboard from source data
pip install python-docx matplotlib
python scripts/build_dashboard.py
```

---

## 📄 Report

A full project report (Word format) with graph explanations, insights, and methodology is available in `report/Urban_Climate_Dashboard_Report.docx`.
