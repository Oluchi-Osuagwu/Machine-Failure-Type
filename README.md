# Machine-Failure-Type

This project aims to develop a classifier that can predict the different modes of failure based on a given set of inputs. The dataset provided consists of 10,000 data points, each represented as a row with 8 features/predictors and a target variable indicating the failure type.

### Dataset
The dataset contains the following columns:

UID: A unique identifier ranging from 1 to 10,000.
productID: A combination of a letter (L, M, or H) representing low, medium, or high product quality variants, and a variant-specific serial number.
Type: Machine type, represented by three categories: H, M, and L.
air temperature [K]: The air temperature in Kelvin.
process temperature [K]: The temperature generated during drilling in Kelvin.
rotational speed [rpm]: The rotational speed in revolutions per minute.
torque [Nm]: The torque values for the drilling process.
tool wear [min]: The amount of time the tool has been used in minutes, indicating tool wear.
Failure Type: The target variable indicating the type of failure.

**Data Preprocessing:** Necessary preprocessing steps were applied to the dataset. This included handling missing and duplicate values and outliers.
Exploratory data analysis (EDA) was done for visualization and gaining of more insights on the dataset and understand the relationships between variables.

**Feature Engineering:** Encoded categorical variables, checked for correlation of features and performed feature scaling. 

**Model Development:** Three machine learning algorithms were considered for the classifier construction, including KNN, random forests and decision trees. The models were trained and evaluated to identify the best-performing one. Resampling was done on the training dataset using SMOTETomek technique. 
The selected models were trained on the resampled training set using the chosen predictors. The trained models were then evaluated using suitable evaluation metrics such as accuracy, precision, recall, and F1-score. 
Model performance was further improved through hyperparameter tuning. Grid search technique was applied to identify the optimal combination of hyperparameters for the chosen models. Cross-validation techniques, k-fold cross-validation, was employed to assess model performance and stratified kfold cross validation was used to further evaluate the model performance.

