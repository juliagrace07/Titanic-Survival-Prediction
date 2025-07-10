# Titanic-Survival-Prediction

This project uses a Random Forest Classifier to predict whether a passenger on the Titanic would survive based on simple input features such as passenger class, age, and gender.

-> Overview
Using the historical Titanic dataset, this project:

Preprocesses the data (including handling missing values and encoding categorical variables)

Trains a Random Forest model

Accepts user input for prediction

Outputs whether the passenger would have survived or not survived

-> Dataset
File: Titanic-Dataset.csv

Assumed columns include at least:

Survived (target: 1 = Survived, 0 = Did not survive)

Pclass (passenger class)

Age

Sex

-> Make sure the CSV file is placed in the same directory as the script.

-> Requirements
Install required Python packages (if not already installed):

bash
Copy
Edit
pip install pandas scikit-learn

-> How It Works
Data Preprocessing

Loads the Titanic dataset

Fills missing values in the Age column using the mean

Encodes the Sex column into a numerical format using one-hot encoding

Model Training

Trains a RandomForestClassifier on the features: Pclass, Age, and Sex

Prediction

Takes user input for passenger class, age, and sex

Predicts survival based on trained model

Prints the result: "Survived" or "Not Survived"

-> Sample Usage
mathematica
Copy
Edit
Enter Pclass (1, 2, or 3): 2  
Enter Age: 25  
Enter Sex (male or female): female  
Prediction: Survived

-> Notes
One-hot encoding is used for the Sex column, keeping only the Sex_male column (i.e., Sex_female is implied).

fillna() is used to handle missing age values by filling them with the mean of the column.

This is a simple implementation focused on demonstrating core ML concepts, not hyperparameter tuning or advanced feature engineering.

 -> Future Enhancements
Add more features like Fare, SibSp, Embarked, etc.

Improve preprocessing (e.g., impute missing values with age-specific strategies)

Hyperparameter tuning using grid search or random search

Build a web interface for easier user interaction (e.g., using Streamlit)

 -> Author
Julia Grace Muddada
Email- juliagrace424@gmail.com
Linkedin- www.linkedin.com/in/julia-grace-muddada-6708271b3
