# 🌤️ Lahore Hourly Weather Data (2020–2025)

An end-to-end data engineering project — fetching, cleaning, feature engineering, and visualizing 5 years of hourly weather data for Lahore, Pakistan using a real REST API.

---

## 📌 Project Overview

This project demonstrates a complete data pipeline:

1. **Data Collection** — Fetched 5 years of hourly weather data from the Open-Meteo Archive API
2. **Data Cleaning** — Handled nulls, removed duplicates, fixed data types
3. **Feature Engineering** — Extracted time features, added season and weather description columns
4. **Exploratory Data Analysis** — Visualized temperature trends, rainfall patterns, and seasonal distributions

---

## 📊 Dataset Summary

| Property | Value |
|---|---|
| Source | Open-Meteo Archive API |
| Location | Lahore, Pakistan (31.5497°N, 74.3436°E) |
| Time Range | 2020-01-01 to 2025-01-01 |
| Frequency | Hourly |
| Rows | 43,872 |
| Columns | 12 |

---

## 📁 Columns

| Column | Description | Unit |
|---|---|---|
| `time` | Datetime of observation | datetime |
| `temperature_2m` | Temperature at 2m height | °C |
| `relative_humidity_2m` | Relative humidity | % |
| `precipitation` | Rainfall amount | mm |
| `wind_speed_10m` | Wind speed at 10m | km/h |
| `weathercode` | WMO weather condition code | - |
| `year` | Extracted year | - |
| `month` | Extracted month | - |
| `day` | Extracted day | - |
| `hour` | Extracted hour | - |
| `season` | Season (Winter/Spring/Summer/Autumn) | - |
| `weather_description` | Human readable weather condition | - |

---

## 📊 Data Visualizations

### Monthly Temperature
![Monthly Temperature](./images/monthly_temperature.png)

### Rainfall Trend
![Rainfall Trend](./images/rainfall_trend.png)

### Season Boxplot
![Season Boxplot](./images/season_boxplot.png)

### Weather Condition
![Weather Condition](./images/weather_condition.png)

## 🛠️ Tools & Technologies

- **Python** — core language
- **Pandas** — data cleaning and feature engineering
- **Matplotlib & Seaborn** — data visualization
- **REST API** — Open-Meteo Archive API
- **Jupyter Notebook** — development environment

---

## 🚀 How to Run

```bash
# Install dependencies
pip install requests pandas matplotlib seaborn

# Run the notebook
jupyter notebook weather_analysis.ipynb
```

---

## 📂 Project Structure

```
├── weather_analysis.ipynb   # Main Jupyter notebook
├── weather_data_cleaned.csv # Final cleaned dataset
└── README.md                # Project documentation
```

---

## 🔗 Links

- 📦 Kaggle Dataset: [Lahore Hourly Weather Data 2020-2025](#)
- 👤 LinkedIn: [Your LinkedIn Profile](#)

---

## 📜 License

Dataset is published under **CC0 (Public Domain)** — free to use for any purpose.
