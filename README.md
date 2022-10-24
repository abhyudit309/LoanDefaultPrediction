# LoanDefaultPrediction
The dataset consists of the following details on loans taken by different customers:  

• ID: A unique identifier for every financial loan that is being considered.

• Loan type: Type of loan taken (Two types, ‘A’ or ‘B’).

• Occupation type: Occupation of the customer (Three occupation types, ‘X’, ‘Y’, ‘Z’).

• Income: A continuous variable that is indicative of the annual income of the customer. This is not the exact income value.

• Expense: A continuous variable that is indicative of the annual expense of the customer. This is not the exact expense value.

• Age: Age of customer – Value of ‘0’ is considered as below 50, and value of ‘1’ is considered as above 50.

• Score1, Score2, Score3, Score4, Score5: Represents five different metrics calculated by the organization, about the customer and the loan that is being considered.

• Label: ‘0’ means non-default, and ‘1’ means default on that loan.

Using the above information and the data, we built models that predict whether a loan will go default or not, and to understand which of the features are important and helpful in the prediction. The dataset has been split into training and test sets. The 'data' folder contains the CSV files for train_x, train_y, and test_x. The train_y file consists of the “Label” that is mentioned above, and train_x consists of the other features. 
A total of 9 models were experimented with, which include
1. Support Vector Machines (4 kernel types)
2. Random Forests
3. Linear Discriminant Analysis
4. Quadratic Discriminant Analysis
5. Boosting Classifier
6. Logistic Regression
7. XGBoost Model
8. Neural Network Model
