# uber-fare-analysis-powerbi
Power BI project analyzing Uber Fares dataset
# Uber Fares Dataset Analysis – Power BI Project

## Overview
This project explores the Uber Fares dataset to identify patterns in fare behavior, ride timing, and peak usage. The dataset was analyzed using Python for data preparation and Power BI for dashboard development and interactive visualization.

---

## Tools Used
- **Python (Pandas):** Data loading, cleaning, and feature engineering
- **Power BI:** Data visualization and interactive dashboard creation
- **GitHub:** Project documentation and version control

---

## Data Processing Steps
The raw Uber dataset was cleaned and transformed using Python:

- Loaded the dataset into a Pandas DataFrame using `pd.read_csv()`
- Removed missing values and filtered outliers (e.g., negative fares or zero-distance trips)
- Applied the **Haversine formula** to calculate `trip_distance` using pickup and drop-off coordinates
- Extracted **hour**, **day**, **month**, and **day_of_week** from the `pickup_datetime`
- Created a **Peak/Off-Peak** indicator for time-based ride segmentation
- Exported the enhanced dataset (`uber_enhanced.csv`) for use in Power BI

---

##  Dashboard Analysis & Insights

### Fare Patterns by Hour, Day of Week, and Month
Time-based visualizations revealed that:
- Fare amounts **peak during 7–9 AM and 4–7 PM**, indicating daily commute patterns.
- **Friday and Sunday** typically have the highest average fares.
- Monthly analysis shows minor fluctuations, suggesting demand is influenced more by **hour and weekday** than season.

### Peak vs Off-Peak Analysis
By comparing peak hours to off-peak:
- **Ride volume is much higher** during peak hours.
- **Average fare amounts** are also slightly higher during peaks, likely due to demand and traffic congestion.
- This validates the importance of dynamic pricing strategies and scheduling driver availability accordingly.

### Hourly, Daily, and Monthly Ride Volumes
- Most rides happen during **weekday peak hours**
- **Sunday rides**, though fewer, tend to have **higher average fares**, likely longer leisure or airport trips.
- Daily and hourly ride count visualizations help pinpoint **high-demand periods** for operational planning.

---

## Key Observations
- Time-of-day is the **strongest driver of fare and ride trends**
- Weekends, especially **Sundays**, have **fewer but more expensive** rides
- **Peak period analysis** shows increased volume and pricing opportunities
- These insights can guide Uber's **driver distribution, marketing strategies, and time-based promotions**

---

## Recommendations
- **Increase driver availability** during peak hours to meet demand
- Offer **off-peak discounts** to encourage ride usage outside rush hours
- Use ride pattern trends to guide **targeted marketing** and **incentive programs**

---

## Project Files
- `uber_cleaned.csv` – Raw data with null values and outliers removed
- `uber_enhanced.csv` – Cleaned dataset with engineered features
- `dashboard.pbix` – Final Power BI interactive dashboard

---


---

## 🖼️ Additional Documentation

The screenshots documenting data loading, cleaning, and dashboard development are included in the following file:  
🔗 [View Screenshots PDF](./screenshots.pdf)

---

## 👤 Author
**Kabucye Kelly** (Student ID: 27113)  
Group A – Introduction to Big Data Analytics (INSY 8413)  
📧 kel.kabucye@gmail.com

## 📘 Instructor
**Eric Maniraguha**  
Lecturer – AUCA  
📧 [eric.maniraguha@auca.ac.rw](mailto:eric.maniraguha@auca.ac.rw)


