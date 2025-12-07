# 🚓 Police Shootings in the USA Analysis & Prediction

## 📌 Project Overview
This project provides a comprehensive data analysis and machine learning pipeline focused on fatal police shootings in the United States (2015-2024). The goal is to uncover patterns related to demographics, geography, and socioeconomic factors, and to build a predictive model for identifying incidents involving mental illness.

The project involves data cleaning, merging with census data (income, poverty, education), exploratory data analysis (EDA), and a classification model.

## 📂 Project Structure
The repository consists of three main Jupyter Notebooks:

### 1. 🧹 Data Cleaning (`CleaningV4.ipynb`)
* **Data Integration:** Merged the main shootings dataset with external census data:
    * Median Household Income
    * Poverty Levels
    * High School Completion Rates
    * Racial Demographics by City
* **Advanced Cleaning:** Used `RapidFuzz` for fuzzy string matching to standardize city names and map them correctly to census data.
* **Imputation:** Handled missing values in age, race, and fleeing status using statistical methods (median/mode).

### 2. 📊 Exploratory Data Analysis (`Q_Analaysis_V2.ipynb`)
An in-depth analysis answering key questions, including:
* **Temporal Trends:** Are incidents increasing over time? (Yearly/Monthly analysis).
* **Geography:** Which states and cities have the highest rates? (Focus on South and West regions).
* **Demographics:** Analysis of victims by Age, Race, and Gender.
* **Threat Analysis:** Breakdown of armed vs. unarmed victims and threat levels.
* **Socioeconomic Factors:** Correlation between poverty/income levels and incident frequency.
* **Key Findings:**
    * Black victims appear at disproportionately higher rates in certain major cities compared to their population share.
    * The "South" region recorded the highest number of incidents.
    * Analysis of "Minimal Threat" incidents over time.

### 3. 🤖 Machine Learning Model (`Prediction_Model.ipynb`)
* **Objective:** Predict whether a victim showed **signs of mental illness** based on incident characteristics.
* **Features Used:** `age`, `gender`, `armed`, `race`, `flee`.
* **Model:** Random Forest Classifier.
* **Technique:** Implemented **SMOTE** (Synthetic Minority Over-sampling Technique) to handle class imbalance in the dataset.
* **Performance:** Achieved an accuracy of ~77% on the test set.

## 🛠️ Tools & Technologies
* **Python 3.x**
* **Data Manipulation:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn, Imbalanced-learn (SMOTE)
* **Text Processing:** RapidFuzz, Unidecode

## 🚀 How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Mohamed-anwer30/Police-Shooting-in-USA.git](https://github.com/Mohamed-anwer30/Police-Shooting-in-USA.git)
    cd Police-Shooting-in-USA
    ```

2.  **Install dependencies:**
    It is recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the Notebooks:**
    Start with `CleaningV4.ipynb` to generate the clean datasets, then proceed to the analysis or prediction notebooks.
    ```bash
    jupyter notebook
    ```

## 📈 Dashboard / Visuals
<img width="1322" height="741" alt="Screenshot 2025-12-07 165414" src="https://github.com/user-attachments/assets/7272e4ce-242d-4c1d-9b0f-16a7fdc51943" />
<img width="1315" height="736" alt="Screenshot 2025-12-07 164833" src="https://github.com/user-attachments/assets/21f31bb3-8514-4741-b46e-5be872a038ee" />
<img width="1319" height="744" alt="Screenshot 2025-12-07 164851" src="https://github.com/user-attachments/assets/663751dc-6887-4ba6-92f8-9b5baa3145c4" />
<img width="1314" height="742" alt="Screenshot 2025-12-07 164906" src="https://github.com/user-attachments/assets/fed78b1b-e06c-467a-9d3e-b61af005587f" />
<img width="1231" height="636" alt="Screenshot 2025-12-07 165008" src="https://github.com/user-attachments/assets/8ef5d688-1add-4804-a474-02c2073310db" />




---
**Author:** Mohamed Anwer
*Certified Data Analyst (MCIT)*
