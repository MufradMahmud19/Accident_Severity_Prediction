# 🚗 Accident Severity Prediction

This repository contains the code and analysis for a project developed as part of the **Big Data Processing and Analytics** course (Master's level). The project explores a large-scale road accident dataset from the United States using PySpark. It focuses on understanding accident patterns, identifying key risk factors, performing spatial analysis, and building a machine learning model to predict accident severity.

---

## 📁 Project Structure
```bash
accident-severity-prediction/                     
|── data/
│   ├── Final_Dataset.csv                                        # Pre-processed and feature engineered dataset
├── notebooks/
│   ├── Feature_Engineering+EDA+Spatial_Analysis.ipynb           # Feature Engineering + Exploratory Data Analysis + geospatial analysis & clustering
│   └── ML_Model_Training.ipynb                                  # Model implementation & evaluation
│
├── figures/
│   
├── report/
│   └── Final_Report.pdf              # Project report (LaTeX output)
├── requirements.txt                  # Python dependencies
├── .gitignore                        # Files to ignore in Git
└── README.md                         # Project overview
```

---

## 🧠 Project Goals

- Analyze temporal and spatial patterns in US road accidents.
- Engineer useful features like accident duration and rush hour indicators.
- Identify accident hotspots through geospatial clustering.
- Build a predictive model to classify accident severity levels.
- Extract actionable insights to inform safety policies.

---

## 🛠️ Tools & Technologies

- **PySpark (Google Colab T4 GPU Runtime)**
- **Matplotlib, Seaborn** – for visualizations
- **KMeans Clustering** – spatial hotspot detection
- **MLlib** – logistic regression-based severity classification
- **Git, LaTeX, Markdown**

---

### About handling the Dataset

Due to file size limitations, the preprocessed `Final_Dataset.csv` is **not included** in this repository.

To reproduce the dataset locally:

1. Download the **raw accident dataset** from [Kaggle](https://www.kaggle.com/code/devbilalkhan/geospatial-insights-us-car-accidents/input).
2. Run the [`notebooks/Feature_Engineering_+_EDA.ipynb`](notebooks/Feature_Engineering_+_EDA.ipynb) notebook to:
   - Clean the data  
   - Perform feature engineering  
   - Generate the final processed dataset
3. Save the output as `Final_Dataset.csv` inside the `data/` folder.

> ⚠️ Ensure you maintain the folder structure as outlined in the project for seamless execution.


## 🔍 Key Highlights

- Engineered time-based features revealed strong behavioral trends in accidents.
- Clustering and heatmaps exposed high-risk geographic zones.
- Severity prediction model provided moderate accuracy and helped identify key influencing variables like weather and distance.
- COVID-19 lockdowns created visible dips in accident trends across years.

---

## 📊 Visualizations

- Hourly and daily accident trends  
- Heatmaps by weekday and hour  
- Severity vs distance scatter plot  
- Geospatial clustering of accidents  
- Correlation heatmap and outlier detection

All figures are available in the `/images` folder.

---


## 📌 How to Run

1. Clone the repository  
   ```bash
   git clone https://github.com/<your-username>/accident-severity-prediction.git
   cd accident-severity-prediction
   ```

2. Open notebooks in Google Colab or Jupyter.

3. Install required dependencies:
```bash
pip install -r requirements.txt
```

4. Follow the notebook flow:

- Feature_Engineering_+_EDA.ipynb

- Spatial_Analysis.ipynb

- ML_Model_Training.ipynb

## 📚 Acknowledgments

- Kaggle US Accidents Dataset: (https://www.kaggle.com/code/devbilalkhan/geospatial-insights-us-car-accidents/input)

- CSC Noppe Jupyter Platform (initial analysis environment)

- Google Colab (for scalable analysis)
