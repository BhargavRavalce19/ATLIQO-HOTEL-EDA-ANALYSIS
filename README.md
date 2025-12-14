# AtliQ Hotels Data Analysis Project

## 📌 Project Overview
This project performs an extensive Exploratory Data Analysis (EDA) on the booking data of **AtliQ Hotels**, a luxury hotel chain in India. The goal is to analyze customer booking behaviors, room occupancy rates, and revenue generation to provide actionable insights for business growth.

## 🛠️ Technologies Used
- **Python**: Core programming language.
- **Pandas**: For data manipulation, cleaning, and aggregation.
- **Matplotlib**: For data visualization (bar charts, etc.).
- **Jupyter Notebook**: Interactive environment for analysis.

## 📂 Dataset
The analysis is based on 5 CSV files located in the `datasets` folder:
1.  `dim_date.csv`: Dates, week numbers, and day types (Weekend/Weekday).
2.  `dim_hotels.csv`: Hotel property details (ID, Name, Category, City).
3.  `dim_rooms.csv`: Room category definitions (RT1, RT2, RT3, RT4).
4.  `fact_aggregated_bookings.csv`: Aggregated booking data (Successful bookings, Capacity).
5.  `fact_bookings.csv`: Transactional booking data (Booking dates, status, revenue, ratings).

## 📊 Analysis Workflow
The project follows a structured data analysis pipeline:

### 1. Data Import & Exploration
- Loading datasets into Pandas DataFrames.
- Exploring data structure, unique values, and statistical summaries.

### 2. Data Cleaning
- **Invalid Guests**: Removing booking records with `no_guests <= 0`.
- **Outlier Handling**: analyzing revenue distribution to check for anomalies (found valid).

### 3. Data Transformation
- **Occupancy Percentage**: Calculated as `(successful_bookings / capacity) * 100`.
- Merging datasets to enrich booking data with hotel and date information.

### 4. Key Insights Generated
The analysis answers critical business questions:
- What is the average **occupancy rate** per room category?
- Which **city** has the highest occupancy and revenue?
- How does occupancy compare between **weekdays** and **weekends**?
- What is the **revenue realized** per city and hotel type?
- Monthly revenue trends.

  <p align="center">
  <img src="screenshots/picture_1.png" width="45%" />
  <img src="screenshots/picture_2.png" width="45%" />
  <img src="screenshots/picture_3.png" width="45%" />
  <img src="screenshots/picture_4.png" width="45%" />
  <img src="screenshots/picture_5.png" width="45%" />
   <img src="screenshots/picture_6.png" width="45%" />
</p>

## 🚀 How to Run
1.  Ensure you have Python installed with the required libraries:
    ```bash
    pip install pandas matplotlib
    ```
2.  Launch Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3.  Open `hotels_analysis.ipynb` and run the cells sequentially.

## 📝 Conclusion
This analysis helps in understanding the performance of different hotel categories and cities, allowing stakeholders to make data-driven decisions to optimize pricing and inventory.
