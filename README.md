# Anomaly Detection and Outlier Analysis in the RITA Dataset

This project explores **anomaly detection and outlier analysis** in the 2019 flight performance data from the **RITA Dataset (Reporting Carrier On-Time Performance)**. By leveraging advanced machine learning techniques, we identify unusual patterns, delays, and operational irregularities in flight operations. The goal is to enhance decision-making and optimize resource allocation in the aviation industry.

---

## **Project Overview**

### **Introduction**
Flight delays significantly impact customer satisfaction and operational efficiency. Using the 2019 RITA dataset, this project focuses on identifying anomalies in flight operations, such as unexpected delays and irregularities. The dataset contains detailed information about flight departures, arrivals, and delays.

---

## **Dataset Details**
- **Source:** RITA Dataset - Reporting Carrier On-Time Performance
- **File Used:** `Flights1_2019_1.csv`
- **Size:** 583,985 rows and 18 columns
- **Variables Analyzed:**
  - `DEP_DELAY` (Departure Delay)
  - `ARR_DELAY` (Arrival Delay)
  - `ORIGIN_AIRPORT_ID` (Origin Airport)
  - `DEST_AIRPORT_ID` (Destination Airport)

---

## **Methodology**
1. **Data Preprocessing:**
   - Handled missing values (3% of the dataset).
   - Focused on the most relevant variables: departure and arrival delays, and airport IDs.

2. **Dimensionality Reduction:**
   - Grouped data by origin and destination airports, reducing the dataset to 5,532 unique origin-destination pairs.

3. **Anomaly Detection Algorithms:**
   Four machine learning algorithms were applied to detect anomalies:
   - **DBSCAN (Density-Based Spatial Clustering of Applications with Noise)**
   - **Isolation Forest**
   - **Local Outlier Factor (LOF)**
   - **One-Class SVM**

4. **Majority Voting Approach:**
   - Combined results of the four algorithms.
   - Classified a data point as an anomaly if at least three out of the four methods agreed.

---

## **Key Findings**
- **22 anomalous trajectories** were identified, primarily due to significant delays in departures or arrivals.
- Anomalies were validated by examining patterns such as peak delays on specific dates or times.
- Visualizations revealed:
  - Delays are more common at departures than at arrivals.
  - Certain days and times exhibit higher delay frequencies.

---

## **Tools and Technologies**
- **Programming Languages:** Python
- **PowerBI is used for the time series ( anomaly detection)**
- **Libraries:** 
  - `pandas` for data manipulation
  - `matplotlib` and `seaborn` for visualization
  - `scikit-learn` for anomaly detection algorithms
- **Visualization Tools:** Box plots, heatmaps, and time series plots.

---

## **Results**
- **Robust Anomaly Detection:** By using a combination of methods, anomalies were detected with high reliability.
- **Insights into Flight Delays:**
  - Flights departing early in the week (e.g., Monday) or during early hours (1-3 AM) exhibited higher delays.
  - Departure delays were generally more significant than arrival delays.

---
To see the report of the project, feel free to reach me at : papemorsylla2201@gmail.com or msyll062@uottawa.ca

**THANK YOU !!!*
