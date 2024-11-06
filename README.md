# MU_PDS-01_Tanzim_PDS_ID_15_Predicting-California-Housing-Prices-with-ML
Overview
This project uses machine learning models to predict house prices in California based on various features such as the average income, housing age, and proximity to the ocean. The project includes the use of two machine learning algorithms:

Linear Regression
Random Forest Regressor
The dataset used is the California Housing Dataset provided by Scikit-learn, which contains information about various districts in California.

Dependencies
This project requires the following Python libraries:

numpy
pandas
scikit-learn
matplotlib
seaborn
To install these dependencies, run:

bash
Copy code
pip install numpy pandas scikit-learn matplotlib seaborn
Dataset
The dataset is the California Housing dataset, which is fetched from Scikit-learn's built-in fetch_california_housing() function. It contains the following features:

MedInc (median income in block group)
HouseAge (median house age in block group)
AveRooms (average number of rooms per household)
AveOccup (average number of occupants per household)
Lat (latitude)
Long (longitude)
MedHouseVal (median house value for California districts)
Other various geographical and housing-related features.
Project Flow
The following steps outline the process of loading the dataset, training models, and evaluating performance.

1. Data Loading and Preprocessing
The dataset is loaded using fetch_california_housing() and is converted into a Pandas DataFrame. The target variable, MedHouseVal (median house value), is separated as the target label, and all other columns are used as features.

2. Data Visualization
Correlation heatmaps are generated using seaborn to understand relationships between features and the target variable.

3. Data Scaling
Features are scaled using StandardScaler to improve model performance. This step is especially important for models like Linear Regression.

4. Model Training and Evaluation
Two machine learning models are trained on the dataset:

Linear Regression: The model is trained, and performance is evaluated using:

Mean Squared Error (MSE)
R-squared (R²) score
Cross-validation to assess model stability.
Random Forest Regressor: A Random Forest model with 100 trees is trained and evaluated similarly.

5. Model Comparison
After evaluating both models, their performances (MSE and R² scores) are compared.

6. Visualization
Scatter plots of predicted vs. actual values are created to visually inspect the performance of the models.
