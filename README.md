Supervised-Machine-Learning
-------

In this example, I use various machine learning techniques to train and evaluate a model based on loan risk. I use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers

Highlights:
-------
* Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
* Split the data into training and testing datasets by using train_test_split
* Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
* Evaluate the model’s performance by doing the following:
* Generate a confusion matrix.
* Print the classification report.

Summary:
-------
Based on the results, both the resampled model and original model show a high level of accuracy and demonstrate good performance in predicting both classes of loan risk. However, after completing an analysis from both models, the resampled model shows slightly higher accuracy (0.994) compared to the first model (0.952). Additionally, the resampled model achieves higher precision, recall, and F1-score for the minority class ("1" class), indicating a better ability to identify high-risk loans.

When determining which model is the best, if the main objective is to achieve overall accuracy and balanced performance for both classes, the resampled model is recommended. It not only achieves high accuracy but also demonstrates improved precision, recall, and F1-score for the high-risk loans. This model would be suitable when both classes ("0" and "1") are equally important.

Likewise, the resampled model more accurately identifies high-risk loans ("1" class), it performs better in terms of precision, recall, and F1-score for the minority class. This can be crucial in situations where correctly identifying high-risk loans is of paramount importance.Considering the slightly higher accuracy and improved performance for the minority class, the resampled model appears to be the preferred choice.

Lastly, we should consider that rather than working with a robust dataset, we are relying on resampling to complete our analysis. We would likely have greater accuracy if we started with a more balanced dataset, and not relied on the resampling. Resampling can artificially balance the dataset, but it does not address the underlying class imbalance issue in the real world. The model's performance may not generalize well to unseen data from the same problem domain, where class imbalance persists. Finding a more balanced dataset from the start can help mitigate these limitations.

It is important to carefully consider the trade-offs between resampling and obtaining a more balanced dataset. If possible, collecting or acquiring a balanced dataset in the first place is preferred. However, if obtaining a balanced dataset is not feasible, resampling techniques can be valuable tools to address class imbalance and improve model performance, while being mindful of their limitations.
