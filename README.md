📁 Titanic Survival Prediction using K-Nearest Neighbors (KNN)
This project builds a machine learning pipeline using the K-Nearest Neighbors (KNN) algorithm to predict whether a passenger survived the Titanic disaster. It includes data preprocessing, feature engineering, hyperparameter tuning, and performance evaluation.

🧠 Model Summary
Algorithm: K-Nearest Neighbors (KNN)

Tuning Method: Grid Search with 5-fold Cross Validation

Evaluation: Accuracy Score and Confusion Matrix

📂 Files
main.py — Main Python script that performs all tasks from loading the dataset to model evaluation and visualization.

tested.csv — Dataset used for model training and testing (preprocessed Titanic dataset).

📊 Features Used
After preprocessing, the following features are used to train the model:

Pclass (Passenger class)

Sex (Converted to 1: Male, 0: Female)

AgeBin (Binned age values)

SibSp, Parch (Number of siblings/spouses and parents/children aboard)

FareBin (Binned fare values)

FamilySize (SibSp + Parch)

IsAlone (1 if traveling alone, else 0)

🔧 Requirements
Install dependencies using pip:

bash
Copy
Edit
pip install pandas numpy scikit-learn matplotlib seaborn
▶️ How to Run
Make sure main.py and tested.csv are in the same directory.

Open terminal or command prompt in that directory.

Run the script:

bash
Copy
Edit
python main.py
📈 Output
Prints the model's accuracy score

Displays the confusion matrix as a heatmap

Automatically tunes the best hyperparameters using GridSearchCV

🔁 Steps Performed
Data Cleaning: Dropping irrelevant columns, filling missing values.

Feature Engineering: Creating FamilySize, IsAlone, and binning Fare and Age.

Preprocessing: Normalizing features using MinMaxScaler.

Model Training: Using KNeighborsClassifier with grid search.

Evaluation: Using accuracy and confusion matrix visualization.

📌 Note on tested.csv
Ensure your tested.csv file contains at least the following columns:

PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

You can download this dataset from Kaggle Titanic Dataset.
