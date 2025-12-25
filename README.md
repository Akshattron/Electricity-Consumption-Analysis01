# ⚡ Electricity Consumption Analysis Tool

## 📊 Project Overview
This project analyzes household electricity consumption data to identify **peak usage patterns** and derive actionable insights for energy optimization.

**Project Type:** Minor 1 - Exploratory Data Analysis (EDA)  
**Difficulty Level:** Medium  
**Completion Date:** December 2025

---

## 🎯 Objectives
- Analyze household electricity consumption data
- Identify peak usage hours and patterns
- Detect anomalies in electricity consumption
- Provide statistical trends and visualizations
- Compare electricity usage across different household areas

---

## 📁 Project Structure
```
Electricity-Consumption-Analysis/
│
├── data/
│   ├── household_power.csv              # Original dataset
│   └── cleaned_household_power.csv      # Cleaned dataset
│
├── notebooks/
│   ├── 01_data_cleaning.ipynb           # Data preprocessing
│   ├── 02_eda_analysis.ipynb            # Exploratory data analysis
│   └── 03_advanced_analysis.ipynb       # Peak usage & advanced analysis
│
├── results/
│   └── graphs/                          # All generated visualizations
│
└── README.md                            # Project documentation
```

---

## 🛠️ Technologies Used
- **Python 3.8**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computations
- **matplotlib** - Data visualization
- **seaborn** - Statistical graphics
- **statsmodels** - Time series analysis

---

## 📊 Dataset Information
- **Source:** UCI Machine Learning Repository - Individual Household Electric Power Consumption
- **Records:** 2,075,259 measurements
- **Time Period:** December 2006 to November 2010 (47 months)
- **Frequency:** 1-minute intervals
- **Features:**
  - Global_active_power: Total active power (kilowatts)
  - Global_reactive_power: Total reactive power (kilowatts)
  - Voltage: Voltage (volts)
  - Global_intensity: Current intensity (amperes)
  - Sub_metering_1: Kitchen (watt-hours)
  - Sub_metering_2: Laundry (watt-hours)
  - Sub_metering_3: Water heater & AC (watt-hours)

---

## 🔬 Analysis Workflow

### 1️⃣ Data Cleaning (`01_data_cleaning.ipynb`)
- Loaded raw dataset with 2M+ records
- Handled missing values (replaced '?' with NaN)
- Converted data types to appropriate formats
- Created DateTime index for time-series analysis
- Removed invalid/incomplete records
- **Output:** Clean dataset ready for analysis

### 2️⃣ Exploratory Data Analysis (`02_eda_analysis.ipynb`)
- Statistical summary of all features
- Distribution analysis of power consumption
- Daily, weekly, and monthly consumption trends
- Sub-metering comparison (household areas)
- Correlation analysis between electrical features
- Voltage stability analysis
- **Output:** 8 comprehensive visualizations

### 3️⃣ Advanced Analysis (`03_advanced_analysis.ipynb`)
- Peak usage hours identification
- Day vs Hour heatmap analysis
- Day of week consumption patterns
- Anomaly detection (unusual high consumption)
- Rolling mean trend analysis
- Seasonal decomposition
- Monthly peak analysis
- Sub-metering peak comparison
- **Output:** 10 advanced visualizations + summary report

---

## 🔥 Key Findings

### ⚡ Peak Usage Patterns
- **Peak Hour:** [20:00 (8 PM)] with average consumption of [1.90 kW] kW
- **Lowest Hour:** [04:00 (4 AM)] with average consumption of [~0.45 kW] kW
- **Peak Day:** [Saturday followed by sunday] shows highest average consumption
- **Peak Month:** [January records maximum average electricity usage, while February holds the record for the single highest peak event] records maximum electricity usage

### 📊 Statistical Insights
- Average electricity consumption: [~1.09 - 1.1 kW] kW
- Maximum recorded consumption: [11.1 kW] kW
- Anomalies detected: [106,882] unusual consumption events

### 🏠 Household Area Analysis
- **Kitchen (Sub_metering_1):** [~1.1] Wh average
- **Laundry (Sub_metering_2):** [Sub_metering_2] Wh average
- **Water Heater & AC (Sub_metering_3):** [~6.5] Wh average
- **Highest consumer:** [Water Heater & AC]

### 📈 Trends Observed
- Clear daily patterns with peaks during [evening from 6 PM to 9 PM] hours
- Weekend vs weekday usage shows [higher consumption on Weekends compared to weekdays.]
- Seasonal variations indicate [higher] consumption in [winter]
- Strong correlation between active power and intensity

---

## 📊 Visualizations Generated

### From EDA Notebook:
1. Distribution of Global Active Power
2. Daily Average Electricity Consumption
3. Monthly Electricity Consumption Trend
4. Sub-Metering Comparison
5. Box Plot for Power Consumption
6. Correlation Heatmap
7. Weekly Consumption Pattern
8. Voltage Analysis

### From Advanced Analysis Notebook:
1. Hourly Consumption Pattern
2. **Peak Hours Analysis** ⭐ (Key deliverable)
3. Day of Week Analysis
4. **Day vs Hour Heatmap** ⭐⭐ (Most important!)
5. Top 10 Peak Consumption Hours
6. Rolling Mean Trend Analysis
7. Anomaly Detection
8. Monthly Peak Analysis
9. Seasonal Decomposition
10. Sub-Metering Peak Analysis

---

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn statsmodels
```

### Execution Steps
1. Clone this repository
2. Place `household_power.csv` in the `data/` folder
3. Open Google Colab or Jupyter Notebook
4. Run notebooks in order:
   - First: `01_data_cleaning.ipynb`
   - Second: `02_eda_analysis.ipynb`
   - Third: `03_advanced_analysis.ipynb`
5. All visualizations will be saved automatically

### For Google Colab Users
- Upload the dataset when prompted
- All graphs will be saved and can be downloaded
- Use the provided download cells at the end of each notebook

---

## 💡 Recommendations Based on Analysis

1. **Energy Optimization:**
   - Shift high-consumption activities away from peak hours
   - Focus on [20:00 (8 PM)] for maximum savings

2. **Load Management:**
   - Implement time-of-use pricing strategies
   - Schedule appliances during off-peak hours

3. **Anomaly Investigation:**
   - Review [106,882] detected anomalies
   - Check for faulty appliances or unusual events

4. **Area-Specific Actions:**
   - [Water Heater & AC] shows maximum usage
   - Consider energy-efficient alternatives for this area

---

## 📥 Dataset Download
The dataset is too large for GitHub. Download it from:
- **Source:** [UCI ML Repository - Individual Household Electric Power Consumption](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- **Direct Download:** [household_power_consumption.zip](https://archive.ics.uci.edu/ml/machine-learning-databases/00235/household_power_consumption.zip)
  

## 📝 Lessons Learned
- Time-series data requires careful preprocessing
- Missing value handling is crucial for accurate analysis
- Rolling means help identify long-term trends
- Heatmaps effectively visualize multi-dimensional patterns
- Anomaly detection reveals unusual consumption events

---

## 🎓 Academic Context
- **Course:** AI/ML Minor Project
- **Semester:** [3rd Semester(CSE Core)]
- **Institution:** [Rungta College of Engineering and Technology]
- **Submission:** December 2025

---

## 👤 Author
**[Akshat Sahu]**
- Email: [akshatsahu1608@gmail.com]
- GitHub: [/Akshattron]

---

## 📚 References
1. UCI Machine Learning Repository - Individual Household Electric Power Consumption Dataset
2. Pandas Documentation: https://pandas.pydata.org/
3. Matplotlib Documentation: https://matplotlib.org/
4. Seaborn Documentation: https://seaborn.pydata.org/
5. Statsmodels Documentation: https://www.statsmodels.org/

---

## 📄 License
This project is created for educational purposes as part of academic coursework.

---

## 🙏 Acknowledgments
- Thanks to my tutor for project guidance
- UCI ML Repository for providing the dataset

---

**⭐ If you found this analysis helpful, please star this repository!**
