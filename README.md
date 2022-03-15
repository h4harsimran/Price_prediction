# Price_prediction
My submission to 30 Days of ML Price prediction competition on kaggle using XGBoost, Custom encoding, Kfold validation, Feature importance.

The jupyter file reads training and testing dataset from the input folder. Data is pre-processed to remove missing values and treat outliers using IQR (Interquartile range method) and capping.

A custome encoding fucntion was defined to reduce the number of unique values in high cardinality columns which help in reducing complexity of the model.

Optimum parameters for XGBoost regressor were found using seprate notebook with Bayesian Optimization.

A five fold cross validation is used to find the best model based on lowest RMSE on test set available.

Feature importance graph is plotted to find which feature have more weight in predicting the target prices. Since the feature were artificially generarted for this competetion and had no real meaning, this graph may not be much useful here but will provide valuable infromation in practical problems.

The submission file was created and submitted to the competetion. The model was able to provide 71% accuracy on the testing set not available to public.
