#  YouTube Trending Video Engagement Analysis

## Overview

This project analyzes YouTube trending videos from the **United States, India, and Canada** to identify factors that influence audience engagement. The analysis combines **Python** for data preprocessing and statistical analysis with **Power BI** for interactive visualization.

The project investigates how **video category**, **title length**, and **country** relate to engagement rates and provides data-driven insights for content creators and marketers.

---

## Objectives

* Examine the effect of title length on audience engagement.
* Investigate how video category influences engagement rates.
* Analyze engagement patterns across the USA, India, and Canada.

---

## Dataset

The project uses the **YouTube Trending Video Dataset** available on Kaggle:

https://www.kaggle.com/datasets/datasnaek/youtube-new

The analysis utilizes the datasets for:

* 🇺🇸 United States
* 🇮🇳 India
* 🇨🇦 Canada

Category IDs were mapped to readable category names using the accompanying JSON metadata files.

---

## Data Preprocessing

The following preprocessing steps were performed:

* Verified category mappings across datasets.
* Combined datasets from the USA, India, and Canada.
* Added country labels for each record.
* Mapped category IDs to descriptive category names.
* Removed duplicate videos while retaining the latest record.
* Removed invalid records with zero views.
* Engineered the following features:

  * Engagement Rate_(%)
  * Title Length (Words)
  * Title Length Groups

---

## Exploratory Data Analysis (EDA)

The exploratory analysis included:

* Distribution of Engagement Rate
* Box Plot for Engagement Rate
* Correlation Heatmap

Distribution of Engagement Rate
<img width="933" height="549" alt="image" src="https://github.com/user-attachments/assets/bdd6c98d-354a-41e5-840b-d09d367bc5d5" />

Box Plot for Engagement Rate
<img width="1226" height="434" alt="image" src="https://github.com/user-attachments/assets/723fcb69-3cc0-4bd9-b176-8162cb7cefe5" />

Correlation Heatmap
<img width="540" height="399" alt="image" src="https://github.com/user-attachments/assets/de38eee8-6684-4f5a-a5ab-872c6ed8aa65" />


### Key Observations

* Engagement rates exhibit a right-skewed distribution.
* A small number of highly engaging videos appear as outliers.
* Title length shows a weak negative relationship with engagement, suggesting that shorter titles tend to receive slightly higher engagement.

---

## Statistical Analysis

The following inferential techniques were applied:

* One-Way ANOVA (Video Category vs. Engagement Rate)
* One-Way ANOVA (Country vs. Engagement Rate)
* Tukey HSD Post Hoc Analysis

These tests were used to determine whether observed differences in engagement were statistically significant.

---

## Dashboard

An interactive **Power BI dashboard** was developed to visualize:

* Average Engagement Rate by Category
* Average Engagement Rate by Country
* Engagement by Title Length Group
* Cross-country comparisons
* Summary metrics and insights

### Overview Dashboard
<img width="638" height="361" alt="image" src="https://github.com/user-attachments/assets/8fd56400-7bc1-420c-80fd-3c04c3e93bc9" />


### Cross-Country Insights
<img width="623" height="384" alt="power_bi_dashboard_youtube" src="https://github.com/user-attachments/assets/7aad1ff6-98e4-4c84-bcab-293ec8df9ff1" />

**Note:** The Power BI dashboard file is available upon request.

---

## Key Findings

* Video category has a statistically significant impact on audience engagement.
* Engagement patterns differ significantly across the USA, India, and Canada.
* Canada exhibited the highest average engagement rate among the three countries.
* Shorter titles generally tended to achieve slightly higher engagement.
* Tukey HSD post hoc analysis confirmed statistically significant differences between all country pairs.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Statsmodels
* Jupyter Notebook
* Power BI


---

## Future Improvements

* Explore predictive models for engagement estimation.
* Incorporate additional metadata such as upload timing and channel characteristics.
* Expand the analysis to include more countries and recent datasets.

---

## License

This project is intended for educational and portfolio purposes. The original dataset is publicly available through Kaggle and remains subject to its respective licensing terms.
