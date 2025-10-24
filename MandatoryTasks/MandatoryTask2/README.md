
My objective for this task was to build a machine learning model to y, using w and x. The dataset was given in two parts training and test datasets.

While reviewing the training data after downloading it from Kaggle, I realised that w is constant throughout the dataset. So I thought of performing feature importance after training it with w and x.

I selected the Random Forest Regressor due to its high performance and accuracy. I couldn’t train the model on the complete dataset because my system was hanging, so I trained only on 50000 lines of data.

Once the model was trained, I then started predicting y values for the test dataset. Here also I could predict only 50000 y since my system was hanging.
I checked the model's feature importances attribute after it was trained. The result was:

W = 0

X = 1

This shows that the model was trained only on X.
