# Machine Learning Trading Bot
Improve the existing algorithmic trading system and enhance the existing algorithms trading signal with machine learning that can adopt new data.

There are the steps to do:
    Establish a Baseline Performance

    Tune the Baseline Trading Algorithm

    Evaluate a New Machine Learning Classifier

    Create an Evaluation Report
Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing the training window?
Hint To adjust the size of the training dataset, you can use a different DateOffset value—for example, six months. Be aware that changing the size of the training dataset also affects the size of the testing dataset.
changing the DateOffse value will change the accuracy score,example as belove:
DateOffset(months=6)
              precision    recall  f1-score   support

        -1.0       0.02      0.44      0.04        86
         1.0       0.98      0.56      0.71      3857

    accuracy                           0.56      3943
   macro avg       0.50      0.50      0.38      3943
weighted avg       0.96      0.56      0.70      3943
DateOffset(months=3)
       precision    recall  f1-score   support

        -1.0       0.04      0.43      0.07       161
         1.0       0.96      0.56      0.71      3931

    accuracy                           0.55      4092
   macro avg       0.50      0.49      0.39      4092
weighted avg       0.92      0.55      0.68      4092



Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters, and record the results in your README.md file. Answer the following question: What impact resulted from increasing or decreasing either or both of the SMA windows?


Choose the set of parameters that best improved the trading algorithm returns. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your README.md file.
![cumulative returns](graph.png)

