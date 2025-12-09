Student Placement Prediction using Logistic Regression

A beginner-friendly Machine Learning project where I built a Logistic Regression model to predict whether a student gets placed based on their CGPA and IQ.
This project helped me understand the complete ML pipeline from EDA to deployment — even though it's simple, it marks an important milestone in my ML learning journey.


🚀 Project Overview

The goal of this project is to build a binary classification model that predicts:
Will the student get placed? (1 = Yes, 0 = No)
based on two input features:
CGPA
IQ

This was my first hands-on ML project, and I followed a structured workflow commonly used in real-world ML development.


🧠 Key Concepts I Learned

These are the steps I practiced and implemented:

0. Preprocessing + EDA + Feature Selection

Loaded the dataset using pandas
Checked missing values, data types, and general structure
Visualized patterns between CGPA, IQ, and placement
Identified the final input & output columns

2. Extract Input and Output Columns

X = CGPA + IQ
y = Placement

4. Scale the Feature Values

Used StandardScaler from Scikit-Learn to normalize CGPA & IQ.

6. Train-Test Split

Used train_test_split to divide dataset into training & testing sets.

7. Train the Model

Trained a Logistic Regression classifier:
from sklearn.linear_model import LogisticRegression

8. Evaluate the Model

Calculated accuracy using accuracy_score
Observed model performance on unseen data

9. Deploy / Save the Model

Saved the trained model using pickle:
pickle.dump(model, open('model.pkl', 'wb'))

(Still learning about model deployment, but saving the model was the first step.)


📊 Dataset Sample

The dataset contains 3 columns:

cgpa	iq	placement
6.8	123	1
5.9	106	0
5.3	121	0
7.4	132	1
5.8	142	0

Dataset source: CampusX GitHub.


📘 Files in This Repository

placement_prediction.ipynb → Full Google Colab notebook
model.pkl → Saved Logistic Regression model
placement.csv → Training toy dataset
README.md → Project documentation (this file)


🙏 Credits

This project was completed as part of my Machine Learning learning journey.
I followed a helpful beginner tutorial by CampusX and used the dataset from their GitHub repository.

Tutorial & dataset source: CampusX YouTube channel & GitHub.
Tutorial link: https://www.youtube.com/watch?v=dr7z7a_8lQw&list=PLKnIA16_Rmvbr7zKYQuBfsVkjoLcJgxHH&index=13
