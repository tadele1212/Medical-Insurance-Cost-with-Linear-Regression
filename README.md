# Medical-Insurance-Cost-with-Linear-Regression
This project explores factors influencing medical insurance costs and builds machine learning models to predict insurance charges. It uses data analysis and visualization techniques to understand the dataset, followed by implementing multiple regression models.

 **Dataset Description**

The dataset consists of information about health insurance beneficiaries. The columns include:

- **age**: Age of the primary beneficiary.
- **sex**: Gender of the insurance contractor (female/male).
- **bmi**: Body mass index (kg/m²).
- **children**: Number of dependents covered by insurance.
- **smoker**: Smoking status (yes/no).
- **region**: Residential area in the US (northeast, southeast, southwest, northwest).
- **charges**: Final medical insurance cost.

 **Key Statistics**

- Number of records: 1,338
- Features: 6
- Target variable: `charges`

 **Exploratory Data Analysis (EDA)**

- Distribution of medical charges (skewed; applied natural log transformation for normalization).
- Analysis of charges by region, smoking status, gender, and number of dependents.
- Relationships between age, BMI, and charges, with smoking as a key factor.

 **Visualizations**

- Distribution plots of charges before and after log transformation.
- Bar plots showing total charges by region and charges segmented by smoking status and gender.
- Violin plots highlighting smoking patterns across different groups.
- Correlation heatmap showing relationships between features.

 **Feature Engineering**

- Converted categorical variables (`sex`, `smoker`, `region`) into numerical using LabelEncoder.
- Checked for missing values and found none.

 Machine Learning Models

 1. Linear Regression
   - R² Score: `0.7998`
   - Coefficients: Age, BMI, children, smoking, and region had significant impacts.

 2. RIDGE Regression
   - R² Score: `0.7996`
   - Used to reduce overfitting by adding a penalty for large coefficients.

 3. LASSO Regression
   - R² Score: `0.7998`
   - Emphasized feature selection by shrinking less important features to zero.

 4. Random Forest Regressor
   - Improved performance with ensemble learning.
   - Tuned hyperparameters for better accuracy.

 Libraries Used

- Data Analysis: `pandas`, `numpy`
- Visualization: `matplotlib`, `seaborn`
- Machine Learning: `scikit-learn`



