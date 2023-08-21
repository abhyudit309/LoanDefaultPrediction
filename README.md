# MS4610 Final Project: Loan Default Prediction

See [`Project_Report.pdf`](Project_Report.pdf) for a description of the project implementation.

The dataset consists of the following details on loans taken by different customers:

* ID: A unique identifier for every financial loan that is being considered.
* Loan type: Type of loan taken (Two types, ‘A’ or ‘B’).
* Occupation type: Occupation of the customer (Three occupation types, ‘X’, ‘Y’, ‘Z’).
* Income: A continuous variable that is indicative of the annual income of the customer. This is not the exact income value.
* Expense: A continuous variable that is indicative of the annual expense of the customer. This is not the exact expense value.
* Age: Age of customer – Value of ‘0’ is considered as below 50, and value of ‘1’ is considered as above 50.
* Score1, Score2, Score3, Score4, Score5: Represents five different metrics calculated by the organization, about the customer and the loan that is being considered.
* Label: ‘0’ means non-default, and ‘1’ means default on that loan.

Using the above information and the data, we built models that predict whether a loan will go default or not, and to understand which of the features are important and helpful in the prediction. The dataset has been split into training and test sets. The [`data`](data) folder contains the CSV files [`train_x.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/data/train_x.csv), [`train_y.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/data/train_y.csv), and [`test_x.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/data/test_x.csv). The [`train_y.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/data/train_y.csv) file consists of the “Label” that is mentioned above, and [`train_x.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/data/train_x.csv) consists of the other features. 

A total of 8 models were experimented with, which include:
1. Support Vector Machines (4 kernel types)
2. Random Forests
3. Linear Discriminant Analysis
4. Quadratic Discriminant Analysis
5. Boosting Classifier
6. Logistic Regression
7. XGBoost Model
8. Neural Network Model

We selected the XGBoost Model and the Neural Network Model, which gave us an accuracy of 98.65% and 98.59% respectively. The [`NN Model`](https://github.com/abhyudit309/LoanDefaultPrediction/tree/main/NN%20Model) folder contains a Jupyter notebook named [`MS4610_Project_Neural_Network.ipynb`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/NN%20Model/MS4610_Project_Neural_Network.ipynb), and the predicted labels of the test set from the Neural Network model in a file named [`pred_y_Neural_Network.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/NN%20Model/pred_y_Neural_Network.csv). The [`XGB Model`](https://github.com/abhyudit309/LoanDefaultPrediction/tree/main/XGB%20Model) folder contains 3 Jupyter notebooks named [`Data_Analysis.ipynb`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/XGB%20Model/Data_Analysis.ipynb), [`Dataset_Choice_Using_CV+Validation.ipynb`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/XGB%20Model/Dataset_Choice_Using_CV%2BValidation.ipynb) and [`Model Choice and Parameter Analysis.ipynb`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/XGB%20Model/Model%20Choice%20and%20Parameter%20Analysis.ipynb), and the predicted labels of the test set from the XGBoost model in a file named [`pred_y_XGB.csv`](https://github.com/abhyudit309/LoanDefaultPrediction/blob/main/XGB%20Model/pred_y_XGB.csv).
