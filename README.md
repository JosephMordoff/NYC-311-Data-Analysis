# NYC-311-Data-Analysis

## Overview

This project analyzes New York City 311 service request data to identify patterns in noise complaints across Manhattan. Using the NYC Open Data API, the analysis focuses on trends over time, complaint frequency, and resolution efficiency.

The goal is to better understand when noise complaints occur most frequently and how quickly they are resolved.

---

## Dataset

* **Source:** NYC Open Data (311 Service Requests)
* **Dataset ID:** `erm2-nwe9`
* **Accessed via:** Socrata Open Data API

The dataset includes:

* Complaint type
* Borough
* Timestamps (created and closed dates)
* Complaint descriptors

---

## Methodology

### 1. Data Collection

* Pulled data using the Socrata API
* Filtered for:

  * Borough: Manhattan
  * Complaint Type: Noise
  * Date: After January 1, 2023

### 2. Data Cleaning

* Removed duplicates
* Converted date fields to datetime format
* Exported raw dataset to CSV

### 3. Feature Engineering

Created new variables:

* Year
* Month
* Day of week

### 4. Analysis

* Descriptive statistics
* Temporal trend analysis
* Complaint frequency patterns

### 5. Visualization

* Monthly complaint trends (line chart)
* Average resolution time by month (bar chart)

---

## Key Insights

* Noise complaints show clear variation by month
* Certain times of year have higher complaint frequency
* Resolution times vary depending on complaint volume

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Socrata Open Data API

---

## How to Run

1. Clone the repository:

   ```
   git clone https://github.com/yourusername/nyc-311-noise-analysis.git
   ```

2. Install dependencies:

   ```
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```
   jupyter notebook nyc_311_noise_analysis.ipynb
   ```

---

## Project Structure

```
nyc-311-noise-analysis/
│
├── nyc_311_noise_analysis.ipynb
├── raw_311_data.csv
├── requirements.txt
└── README.md
```

---

This project was developed as part of a data analytics course and demonstrates real-world data collection, cleaning, and visualization using public datasets.
