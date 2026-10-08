# California House Price Prediction
 
An end-to-end machine learning project that predicts California housing prices using demographic, socioeconomic, and geographic features from the California Housing Dataset. The project demonstrates the complete machine learning workflow, including data exploration, visualization, feature engineering, model development, evaluation, and performance improvement using Scikit-Learn pipelines.
 
## Project Overview
 
Housing price prediction is a classic regression problem that can provide valuable insights for real estate analysis, investment decisions, and market forecasting. In this project, machine learning techniques were applied to estimate median house values across California districts.
 
The project focuses on:
 
- Exploratory Data Analysis (EDA)
- Feature correlation analysis
- Data preprocessing
- Regression modeling
- Pipeline implementation
- Feature engineering
- Model evaluation and refinement
 
---
 
## Dataset
 
This project uses the California Housing Dataset available through Scikit-Learn.
 
### Features
 
| Feature | Description |
|----------|-------------|
| MedInc | Median income in block group |
| HouseAge | Median house age |
| AveRooms | Average number of rooms per household |
| AveBedrms | Average number of bedrooms per household |
| Population | Block group population |
| AveOccup | Average household occupancy |
| Latitude | Geographic latitude |
| Longitude | Geographic longitude |
 
### Target Variable
 
**MedHouseValue**
 
The median house value for California districts.
 
---
 
## Key Findings
 
- Median Income (MedInc) showed the strongest positive correlation with house prices.
- Geographic location significantly influences housing values.
- Feature engineering improved model performance considerably.
- Non-linear relationships exist within the housing data and can be captured using polynomial features.
 
---
 
## Project Workflow
 
### 1. Data Collection
 
- Loaded the California Housing Dataset from Scikit-Learn.
- Converted the data into a Pandas DataFrame for analysis.
 
### 2. Exploratory Data Analysis (EDA)
 
- Explored feature distributions.
- Analyzed correlations between variables.
- Identified key predictors of housing prices.
- Investigated geographic patterns.
 
### 3. Data Visualization
 
Created visualizations including:
 
- Feature correlation plots
- Housing value distribution charts
- Geographic housing price maps
- Actual vs Predicted value comparisons
 
### 4. Data Preprocessing
 
- Train-test split
- Feature standardization using StandardScaler
- Pipeline construction
- Polynomial feature engineering
 
### 5. Model Development
 
Built and evaluated multiple regression pipelines to improve predictive performance.
 
---
 
## Machine Learning Pipelines
 
### Baseline Model
 
**Pipeline Components**
 
- StandardScaler
- Linear Regression
 
```python
pipeline = Pipeline([
('scaler', StandardScaler()),
('model', LinearRegression())
])
```
 
#### Performance
 
| Metric | Value |
|----------|----------|
| R² Score | 0.5758 |
| Mean Squared Error (MSE) | 0.56 |
 
---
 
### Enhanced Model
 
**Pipeline Components**
 
- StandardScaler
- PolynomialFeatures
- Linear Regression
 
```python
pipe = Pipeline([
('scale', StandardScaler()),
('polynomial', PolynomialFeatures(include_bias=False)),
('model', LinearRegression())
])
```
 
#### Performance
 
| Metric | Value |
|----------|----------|
| R² Score | 0.6457 |
| Mean Squared Error (MSE) | 0.5559 |
 
---
 
## Results
 
### Model Comparison
 
| Model | R² Score | MSE |
|---------|---------|---------|
| Linear Regression | 0.5758 | 0.5600 |
| Polynomial Regression | 0.6457 | 0.5559 |
 
### Performance Improvement
 
By introducing polynomial feature engineering:
 
- R² score improved from **57.58%** to **64.57%**
- The model captured more complex relationships in the data
- Prediction accuracy increased compared to the baseline model
 
### Visualization
 
Actual and predicted housing values were compared using Kernel Density Estimation (KDE) plots to assess model quality and prediction accuracy.
 
---
 
## Technologies Used
 
### Programming Language
 
- Python
 
### Libraries
 
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- 
## Skills Demonstrated
 
- Machine Learning
- Predictive Modeling
- Regression Analysis
- Exploratory Data Analysis (EDA)
- Data Visualization
- Feature Engineering
- Scikit-Learn Pipelines
- Model Evaluation
- Statistical Analysis
- Python Programming
- Data Preprocessing
- Problem Solving
 
---
 
## Highlights
 
✅ Built an end-to-end machine learning workflow
 
✅ Performed exploratory data analysis and feature correlation studies
 
✅ Developed production-style Scikit-Learn pipelines
 
✅ Improved model performance through feature engineering
 
✅ Increased R² score from **0.5758** to **0.6457**
 
✅ Visualized housing value distributions and geographic trends
 
✅ Demonstrated practical machine learning and data science skills
 
---
 
