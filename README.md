# Water Contamination Risk Analysis in Morocco 💧

**Data-Driven Analysis of Water Sources Across Morocco Using Machine Learning**

---

## Project Overview

Access to clean water is a critical issue in Morocco. This project analyzes water sources across multiple regions and predicts the **risk of contamination** using machine learning techniques.  

The analysis covers:

- Rivers, springs, wells, and shared taps  
- Environmental factors like rainfall, temperature, soil moisture, and nearby agriculture  
- Population served by each water source  
- Contamination risk prediction using a **Random Forest Classifier**

---

## Dataset

The dataset contains 100 records of water sources with the following features:

| Column | Description |
|--------|-------------|
| `source_id` | Unique identifier for each water source |
| `region` | Moroccan region of the water source |
| `source_type` | Type of water source (river, spring, well, shared tap) |
| `avg_rainfall_mm` | Average monthly rainfall in mm |
| `last_rain_days` | Days since last rainfall |
| `pop_served` | Number of people served by the water source |
| `nearby_agriculture` | Whether agriculture is nearby (`yes`/`no`) |
| `temp_c` | Average temperature in °C |
| `soil_moisture` | Soil moisture level (`very_low`, `low`, `medium`, `high`) |
| `contamination_risk` | Target variable: contamination risk (`low`, `medium`, `high`, `very_high`) |

---

## Exploratory Data Analysis (EDA)

- Visualized feature distributions and correlations  
- Handled categorical variables using **Label Encoding**  
- Examined contamination risk across different regions and source types  

---

## Machine Learning Model

- **Model Used:** Random Forest Classifier  
- **Train/Test Split:** 80% / 20%  
- **Hyperparameter Tuning:** GridSearchCV to optimize `n_estimators`, `max_depth`, `min_samples_split`, and `min_samples_leaf`  


**Sample Predictions for New Water Sources:**

| Water Source | Predicted Contamination Risk |
|--------------|-----------------------------|
| Source 1     | low                         |
| Source 2     | high                        |

---

## Geospatial Visualization

A map showing contamination risk across Moroccan water sources:

![Water Contamination Map](images/morocco_contamination_risk_map.png)

*Interactive map created in Folium and saved as a screenshot.*

---

## Key Insights

- Rivers and springs tend to have higher contamination risk in regions with lower rainfall and higher temperatures  
- Nearby agriculture can increase contamination risk for wells and shared taps  
- The model can help authorities prioritize water source improvements and preventive measures  

---

## Technologies Used

- Python 3  
- Pandas, NumPy for data processing  
- Matplotlib & Seaborn for visualization  
- Scikit-learn for machine learning  
- Folium for geospatial visualization  

---

## 🛠️ Tools Used

- Python
- Pandas
- Scikit-learn
- Seaborn & Matplotlib
- Jupyter Notebook

---

## 📬 Contact

Created by **FELLAH HANANE**  
📧 Email: hananefellah35@gmail.com  
🌐 GitHub: [hananefellah](https://github.com/hananefellah)

---

## 📄 License

This project is open-source under the MIT License.

## How to Use

1. Clone this repository:  

```bash
git clone https://github.com/<your-username>/water-contamination-risk-morocco.git
