

---

# Fire Detection and Analysis Using NASA VIIRS Data

## Project Overview

This project focuses on the **analysis of satellite-based fire detection data** using the **NASA Visible Infrared Imaging Radiometer Suite (VIIRS)**. The VIIRS instrument, aboard polar-orbiting satellites, continuously captures data to monitor environmental phenomena, including wildfires. This project analyzes the satellite data to understand fire intensity, detection reliability, and spatial-temporal patterns of fire events.

### Dataset
The dataset contains satellite observations of fire hotspots detected in June, including key features like:
- **Latitude and Longitude**: The geographical location of the fire.
- **Brightness Temperature**: Measured in Kelvin, indicating the heat intensity of the fire.
- **Fire Radiative Power (FRP)**: Measured in megawatts (MW), reflecting the intensity of the fire.
- **Confidence**: The reliability of the fire detection (low, nominal, high).
- **Day/Night Indicator**: Whether the fire was detected during the day or night.

---

## Objective

The goal of this project is to:
1. **Preprocess and clean the data** to handle missing values and duplicates.
2. **Explore key relationships** between variables, including fire intensity and detection confidence.
3. **Analyze spatial and temporal patterns** of fire events.
4. **Visualize insights** to aid in fire management and detection.

---

## Steps Performed

### 1. Data Cleaning and Preprocessing
- **No missing or duplicate data** was found, but steps for handling missing values and duplicates were included as a precaution.
- Converted **date** columns to a datetime format and transformed categorical columns (e.g., **confidence** and **daynight**) into numerical values for analysis.

### 2. Exploratory Data Analysis (EDA)
- **Statistical summaries** revealed important insights, including the wide range of fire brightness temperatures (299K to 367K) and fire radiative power (FRP) from 0.7 MW to 312 MW.
- **Correlation analysis** showed a strong positive relationship between brightness and FRP, confirming that higher brightness indicates stronger fire intensity.

### 3. Visualizations
A series of visualizations were created to explore the dataset:
- **Heatmap of Correlations**: Showed strong correlations between brightness, FRP, and other numerical features.
- **Geographical Scatter Plot**: Visualized fire detections across different geographical locations, highlighting regions with high-intensity fires.
- **Boxplots**: Compared brightness and FRP across different confidence levels, revealing that higher confidence detections correspond to more intense fires.
- **Time Series Plot**: Illustrated fire detections over time, revealing patterns in fire activity throughout the dataset's observation period.

---

## Key Insights

1. **Fire Intensity**:
   - **Brightness** and **FRP** are highly correlated, meaning higher brightness is a reliable indicator of fire intensity. Intense fires, reflected by high FRP, were captured by the dataset, with some extreme cases of FRP exceeding 300 MW.

2. **Confidence Levels**:
   - Most fire detections were of **nominal confidence**, indicating reliable detections. **High confidence detections** were associated with the most intense fires.

3. **Geographical and Temporal Trends**:
   - The **spatial analysis** showed that fires were concentrated in specific regions, likely reflecting areas prone to wildfires. 
   - **Temporal patterns** revealed consistent fire detections both day and night, with some variation in fire activity over time.

---

## Tools and Technologies Used

- **Python**: For data manipulation, analysis, and visualization.
- **Pandas**: For data cleaning and preprocessing.
- **Matplotlib & Seaborn**: For generating insightful visualizations.
- **Jupyter Notebook**: For interactive analysis and code execution.

---

## Conclusion

This project successfully analyzed the **NASA VIIRS fire detection dataset**, providing key insights into **fire intensity**, **detection reliability**, and **spatial-temporal trends**. The insights drawn from this project can help improve **fire detection strategies**, aid in **disaster management**, and inform **resource allocation** for firefighting efforts.

---

## Future Work

- Incorporate additional satellite data to analyze fire trends over longer periods.
- Apply machine learning models for **fire intensity prediction** based on the brightness, FRP, and other variables.
- Extend the geographical analysis to identify **high-risk fire zones** and optimize detection strategies.

---

## Acknowledgments

Special thanks to **NASA** for providing the VIIRS data, and the open-source Python community for the libraries and tools used in this analysis.

---

