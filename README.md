This code is for determination of cardiopulmonary resuscitation(CPR) quality.
I used 3 machine learning algorithm (SVM, KNN, XGBOOST) to classify CPR quality.
I used the gridsearchCV function to find best hyperparamters. 
The hyperparameter of these three models are

SVM = 
1. Total feature model {'C': 1000, 'gamma': 1, 'kernel': 'rbf'}
2. Non-invaisve feature model {'C': 100, 'gamma': 1, 'kernel': 'rbf'}
3. Clinical feature model {'C': 1000, 'gamma': 1, 'kernel': 'rbf'}

KNN =
1. Total feature model {'metric': 'manhattan', 'n_neighbors': 5, 'weights': 'distance'}
2. Non-invaisve feature model {'metric': 'manhattan', 'n_neighbors': 8, 'weights': 'distance'}
3. Clinical feature model {'metric': 'manhattan', 'n_neighbors': 4, 'weights': 'distance'}

XGBOOST = 
1. Total feature model {'colsample_bytree': 1, 'max_depth': 10, 'min_child_weight': 1, 'n_estimators': 300}
2. Non-invaisve feature model {'colsample_bytree': 0.75, 'max_depth': 9, 'min_child_weight': 1, 'n_estimators': 200}
3. Clinical feature model {'colsample_bytree': 0.5, 'max_depth': 7, 'min_child_weight': 1, 'n_estimators': 200}
