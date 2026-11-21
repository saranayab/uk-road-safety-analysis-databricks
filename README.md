# UK Road Safety Data Pipeline (Databricks)

## 📌 Overview

Developed a data processing and analysis pipeline using Databricks, Apache Spark (PySpark) and SQL to investigate UK road accident data from 2020–2024.

Cleaned, transformed, and analysed collision, vehicle, and casualty datasets, performing data validation, feature engineering and aggregation to identify patterns in accident frequency, road conditions, and casualty severity.

Created visualisations to explore road safety trends and communicate analytical findings.

---

## 📂 Dataset

The dataset consists of three main tables:

* **Collisions** – details of each accident (time, location, weather, severity, etc.)
* **Vehicles** – information about vehicles involved
* **Casualties** – details about affected individuals

These tables are linked using a common key: `collision_index`.

---

## ⚙️ Technologies Used

* **Databricks**
* **Apache Spark (PySpark)**
* **Python**
* **SQL (Spark SQL)**

---

## 🔄 Data Pipeline Steps

### 1. Data Preparation

* Renamed original tables for clarity (`collisions`, `vehicles`, `casualties`)
* Removed duplicates
* Handled missing values using default placeholders (-1)

### 2. Data Cleaning

* Filtered invalid or missing values
* Ensured consistency in key variables (time, speed limit, etc.)

### 3. Feature Engineering

* Created new features such as:

  * `hour_of_day`
  * `weather_group`
  * `road_type_label`

### 4. Data Transformation

* Grouped and aggregated data for analysis
* Converted coded variables into readable labels

---

## 📊 Analysis Performed

### Query 1

Analysis of accident frequency across different weather conditions and speed limits.

### Query 2

Impact of speed limits and road types on the number of casualties.

### Query 3

Temporal analysis of accident patterns by hour of day and day of week.

---

## 📈 Visualisation

Visualisations were created within Databricks to support analysis.
Due to platform limitations, some visualisations may not fully render in `.ipynb` format.

👉 An **HTML version (Download it)** of the notebook is included for complete visual output.

---

## ⚠️ Notes

* The `.ipynb` file may be large due to included outputs.
* Some environments (e.g., VS Code or Databricks preview) may not fully render the notebook.
* The HTML file provides a complete and accurate representation of the results.

---

## 📁 Files Included

* `UK-Road-Safety-Data-pipeline.ipynb` – Main notebook
* `UK_Road_Safety.html` – Full output version (recommended for viewing)

---

## 👤 Author

**Sara Nayab Khalid**

