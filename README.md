# ✈️ Flight Delay Prediction

This project explores flight delay patterns using real-world airline data and builds a machine learning model to predict whether a flight will be delayed. The workflow includes end-to-end data analysis, feature engineering, model training, and interpretation—all documented in a Jupyter Notebook.

---

## 🎯 Objectives

- Explore delay trends and variability across airlines, time, and locations.
- Create a binary classifier to predict flight delays (15+ minutes).
- Practice and showcase machine learning skills with a well-structured notebook.
- Use visual storytelling to explain patterns and model findings.

---

## 🧪 Project Workflow

1. **Exploratory Data Analysis (EDA)**
   - Visualized missing data patterns using `missingno`.
   - Identified key delay drivers: departure delay, time of day, carrier, airport.
   - Used box plots and heatmaps to examine variability across airlines.

2. **Feature Engineering**
   - Created `is_delayed` target (1 if arrival delay ≥15 mins, else 0).
   - Converted scheduled time columns into full datetime objects.
   - Extracted components like hour, minute, and weekday for modeling.
   - One-hot encoded categorical variables for airline, airport, etc.

3. **Modeling**
   - Trained two models: `LogisticRegression` and `RandomForestClassifier`.
   - Evaluated using accuracy, precision, recall, and confusion matrices.
   - Random Forest yielded improved delay classification performance (~91% accuracy).

4. **Interpretation**
   - Extracted and visualized top feature importances.
   - Generated follow-up plots to explain how variables like airline and hour relate to delay rate.

---

## 🔍 Key Insights

- **Departure delay** is the strongest predictor of arrival delay.
- **Airline behavior**, **origin airport**, and **hour of day** also significantly influence delay likelihood.
- Box plots revealed that some airlines (e.g., Envoy Air) are more consistent, while others (e.g., Frontier) have higher delay variability.
- Visual EDA and model interpretation combine to offer compelling, transparent insights into aviation delay dynamics.

---

## 🧰 Tools Used

- Python, Jupyter Notebook
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, Missingno, Scikit-learn

---

## 📁 Data Source

This project is based on a real-world flight dataset available from Kaggle:

**[Flight Dataset – 2013](https://www.kaggle.com/datasets/mahoora00135/flights)**

> *Note: The dataset was preprocessed to create a delay label, handle missing values, and engineer datetime features for modeling.*

--- 
---

## 🧠 Author Notes

This project was built with guidance from an AI assistant (Copilot). All code was reviewed, understood, and explained to ensure clear comprehension and honest reflection on the learning process. The goal was not to automate, but to build understanding.

---

## 🚀 Author

**Martin**  
Curious data scientist in training, focused on real-world insights through EDA, visualization, and predictive modeling.

⚠️Note: As my first project, this projecthas been built as a learning exercise, with guidance from an AI assistant (Copilot). Every step—from code to modeling choices—was reviewed, tested, and interpreted personally to ensure full understanding. The project reflects my learning journey into machine learning, not a pre-existing template or auto-generated solution.

## 📦 Project Structure
flight-delay-prediction/ ├── flight_delay__prediction_project.ipynb # Jupyter notebook with code and visuals ├── README.md # Project summary and documentation ├── images/ #  Folder to store saved plots ├── requirements.txt #  File listing Python dependencies





