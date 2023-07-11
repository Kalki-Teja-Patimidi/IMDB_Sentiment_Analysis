# Chennai House Price Prediction
This repository contains code for a machine learning model that predicts house prices in Chennai, India. The model is trained on a dataset of various features related to the houses, such as area, number of bedrooms, number of bathrooms, location, and more.

The goal of this project is to help buyers determine a fair price for a house and provide insights to sellers on what factors can fetch them higher prices for their properties.

Dataset
The dataset used for training the model is stored in the file train-chennai-sale.csv. It contains the following variables:

PRT_ID: Project ID
AREA: Area where the house is located
INT_SQFT: Total area of the house in square feet
DATE_SALE: Date on which the house was sold
DIST_MAINROAD: Distance from the house to the main road (in meters)
N_BEDROOM: Number of bedrooms
N_BATHROOM: Number of bathrooms
N_ROOM: Number of rooms
SALE_COND: Sale conditions
PARK_FACIL: Parking facility availability
DATE_BUILD: Date on which the house was built
BUILD_TYPE: Type of the house
UTILITY_AVAIL: Utilities available for the owner of the house
STREET: Street where the house is located
MZZONE: Chennai regions divided into multiple zones
QS_ROOMS, QS_BATHROOM, QS_BEDROOM, QS_OVERALL: Masked data
REG_FEE: Registration fees
COMMIS: Commission
SALE_PRICE: Price at which the house was sold
Getting Started
To use this code, follow the steps below:

Clone this repository to your local machine.
Install the required dependencies mentioned in the requirements.txt file.
Open the Jupyter notebook Chennai_House_Price.ipynb to access the code.
Run the notebook cells to execute the code and generate the house price predictions.
Preprocessing
The code performs several preprocessing steps on the dataset, including:

Renaming columns to lowercase
Dropping irrelevant columns (PRT_ID, REG_FEE, COMMIS)
Handling missing values by filling them with appropriate statistical techniques
Correcting data types of columns (n_bedroom, n_bathroom, date_sale, date_build)
Creating a new column 'house_age' based on the date_sale and date_build columns
Encoding categorical variables using ordinal encoding and one-hot encoding
Model Building and Evaluation
The code builds and evaluates multiple machine learning models for house price prediction, including:

Linear Regression
K Nearest Neighbors Regression
Decision Tree Regression
Random Forest Regression
Extreme Gradient Boosting Regression
For each model, the code calculates the cross-validation score and R2 score to assess its performance.

Feature Importance
The code also provides insights into the importance of different features in predicting house prices. It uses the Random Forest and Extreme Gradient Boosting models to determine the feature importance and visualizes the results in bar charts.

Suggestions to Sellers and Buyers
Based on the feature importance analysis, the code provides suggestions to sellers and buyers on factors that can influence house prices. Sellers are advised to focus on the following features to build homes that fetch higher prices:

Age of the building
Area (location) of the building
Number of rooms
Build type (commercial properties tend to have higher prices)
MZ zone
Parking facility availability
Number of bedrooms
Area (in square feet) of the building
Number of bathrooms
Street type (paved streets are preferred)
Sale conditions
Utilities available
Conclusion
The Chennai House Price Prediction model can be used by buyers to estimate fair prices for houses and assist sellers in understanding the factors that can fetch higher prices for their properties. The model provides a valuable tool for the real estate market in Chennai, helping both buyers and sellers make informed decisions.

Please feel free to explore the code and adapt it to your specific needs. If you have any questions or suggestions, please open an issue or reach out to the repository owner.

Happy house hunting and selling!
