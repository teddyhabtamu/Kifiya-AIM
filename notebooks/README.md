# Data Analysis for Solar Energy and Weather Data

## Project Overview

This project involves the analysis of solar energy and weather data from three different countries. The analysis includes exploratory data analysis (EDA), data cleaning, and various statistical and visualization techniques to understand the relationships between different variables.

## Notebooks

### 1. Exploratory Data Analysis (EDA) for three different datasets:

- **Summary Statistics**: Calculate mean, median, standard deviation, and other statistical measures for each numeric column to understand data distribution.
- **Data Quality Check**: Look for missing values, outliers, or incorrect entries, especially in columns like GHI, DNI, and DHI. Check for outliers in sensor readings (ModA, ModB) and wind speed data (WS, WSgust).
- **Time Series Analysis**: Plot bar charts or line charts of GHI, DNI, DHI, and Tamb over time to observe patterns by month, trends throughout the day, or anomalies. Evaluate the impact of cleaning (using the 'Cleaning' column) on the sensor readings (ModA, ModB) over time.
- **Temperature Analysis**: Examine how relative humidity (RH) might influence temperature readings and solar radiation.
- **Histograms**: Create histograms for variables like GHI, DNI, DHI, WS, and temperatures to visualize the frequency distribution of these variables.
- **Z-Score Analysis**: Calculate Z-scores to flag data points that are significantly different from the mean.
- **Bubble Charts**: Explore complex relationships between variables, such as GHI vs. Tamb vs. WS, with bubble size representing an additional variable like RH or BP (Barometric Pressure).

### 2. Data Cleaning for three datasets:

- **Identify Missing Values**: Check for missing values in the dataset.
- **Handle Missing Values**: Drop columns that are entirely null (e.g., 'Comments') and fill missing values in numeric columns with the median.
- **Handle Anomalies**: Remove rows with negative values in columns where only positive values are expected.
- **Drop Unnecessary Columns**: Drop columns that are not useful for analysis.

## Data Sources

The data used in this project comes from three different countries. Each dataset includes various columns such as:
- **Timestamp**: The date and time of the observation.
- **GHI**: Global Horizontal Irradiance.
- **DNI**: Direct Normal Irradiance.
- **DHI**: Diffuse Horizontal Irradiance.
- **Tamb**: Ambient Temperature.
- **RH**: Relative Humidity.
- **WS**: Wind Speed.
- **WSgust**: Wind Gust Speed.
- **ModA**: Sensor Reading A.
- **ModB**: Sensor Reading B.
- **BP**: Barometric Pressure.
- **Cleaning**: Indicator for cleaning events.

## How to Use

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/teddyhabtamu/Kifiya-AIM-Week-0.git
2. **Navigate to the Project Directory**:
   ```sh
   cd Kifiya-AIM-Week-0
3. **Install Dependancies**: 
   ```sh
   pip install pandas numpy matplotlib seaborn scipy
4. **Open the Jupyter notebooks and run the cells**


## Results
The analysis provides insights into the relationships between various weather and solar energy variables. Key findings include:

- Patterns and trends in solar irradiance and temperature over time.
- The impact of cleaning on sensor readings.
- The influence of relative humidity on temperature and solar radiation.
- Identification of outliers and anomalies in the data.

## Conclusion
This project demonstrates the importance of data cleaning and exploratory data analysis in understanding complex datasets. The visualizations and statistical analyses provide valuable insights into the behavior of solar energy and weather variables across different countries.
