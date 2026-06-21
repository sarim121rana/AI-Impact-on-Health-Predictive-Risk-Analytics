# 🚀 AI Impact on Health: Predictive Risk Analytics

## 📌 Project Overview
The integration of Artificial Intelligence in healthcare is rapidly changing how we monitor and maintain personal well-being. This project analyzes the effectiveness of various AI health tools (Fitness Trackers, Mental Health Apps, Telemedicine) and builds a robust Machine Learning model to predict a patient's **Health Risk Category (Low, Medium, High)** based on their physical metrics and lifestyle habits.

## 🎯 Business Value & Impact
* **Proactive Healthcare:** Enables early detection of high-risk patients based on easily accessible metrics like BMI and exercise routines.
* **Personalized Recommendations:** Helps health professionals understand which factors contribute most to health risks, allowing for highly targeted interventions.
* **Data-Driven Decision Making:** Transforms raw patient data into actionable insights without the need for immediate, complex medical testing.

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.x
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Random Forest Classifier)
* **Environment:** Google Colab / Jupyter Notebook

## ⚙️ Project Architecture & Workflow

### 1. Data Preprocessing & Cleaning
* Extracted a dataset of 5,000 unique patient records.
* Removed non-predictive identifiers to prevent model confusion.
* Handled missing values and ensured correct data types across all features.

### 2. Exploratory Data Analysis (EDA)
* Conducted univariate analysis to understand the distribution of Age, BMI, and Risk Categories.
* Performed multivariate analysis using correlation heatmaps to discover hidden relationships between lifestyle choices and overall health risk.

### 3. Feature Engineering
* Handled the **Dummy Variable Trap** by converting categorical variables (Gender, Chronic Conditions) into optimized boolean/integer formats (`drop_first=True`) for algorithmic efficiency.
* Encoded the ordinal target variable (`Risk_Category`) into numerical ranks.

### 4. Predictive Modeling
* Split the dataset into an 80/20 Train-Test configuration to ensure unbiased evaluation.
* Deployed an ensemble learning technique using a **Random Forest Classifier** (100 estimators) to capture complex, non-linear relationships in the health data.
* Achieved perfect predictive accuracy on the synthetic dataset.

### 5. Live Prediction System
* Built a custom prediction pipeline that accepts raw user inputs (e.g., Age, BMI, Exercise Hours) and outputs a real-time risk assessment (e.g., 'Low Risk' or 'High Risk').

## 📊 Key Analytical Insights
Through rigorous correlation analysis, the following patterns were identified:
* **The Ultimate Risk Driver:** Pre-existing **Chronic Conditions** showed the strongest positive correlation (0.74) with a High-Risk categorization.
* **The Weight Factor:** **BMI** serves as the second most critical indicator (0.40 correlation). Higher BMI significantly escalates the predicted risk level.
* **Age as a Secondary Variable:** While Age showed a positive correlation (0.26), it acts as a secondary risk multiplier rather than a primary cause compared to lifestyle and medical history.

## 💡 How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have the required libraries installed (`pip install pandas numpy matplotlib seaborn scikit-learn`).
3. Run the Jupyter Notebook cell by cell.
4. Use the `dummy_patient` DataFrame at the end of the notebook to test the model with your own custom health inputs!
