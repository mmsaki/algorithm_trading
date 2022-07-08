# Machine Learning Trading Bot

## Table of Contents

1. Background
2. Instructions
3. Tune the Baseline Trading Algorithm
4. Evaluate a New Machine Learning Classifier
5. Summary

## Background
- Create an algorithmic trading bot that learns and adapts to new data and evolving markets.
- I assume the role of a financial advisor at one of the top five financial advisory firms in the world.
- My firm constantly competes with the other major firms to manage and automatically trade assets in a highly dynamic environment.
- My firm has heavily profited by using computer algorithms that can buy and sell faster than human traders.
- The speed of these transactions gave my firm a competitive advantage early on
- People still need to specifically program these systems, which limits their ability to adapt to new data.
- I am thus planning to improve the existing algorithmic trading systems and maintain the firm’s competitive advantage in the market.
- To do so, i'll enhance the existing trading signals with machine learning algorithms that can adapt to new data.

## Instructions

1. Import the OHLCV dataset into a Pandas DataFrame.

2. Generate trading signals using short- and long-window SMA values.

3. Split the data into training and testing datasets.

4. Use the `SVC` classifier model from SKLearn's support vector machine (SVM) learning method to fit the training data and make predictions based on the testing data. Review the predictions.

5. Review the classification report associated with the `SVC` model predictions.

6. Create a predictions DataFrame that contains columns for “Predicted” values, “Actual Returns”, and “Strategy Returns”.

7. Create a cumulative return plot that shows the actual returns vs. the strategy returns. Save a PNG image of this plot. This will serve as a baseline against which to compare the effects of tuning the trading algorithm.

8. Write your conclusions about the performance of the baseline trading algorithm in the `README.md` file that’s associated with your GitHub repository. Support your findings by using the PNG image that you saved in the previous step.

## Tune the Baseline Trading Algorithm

* Tune the training algorithm by adjusting the size of the training dataset. To do so, slice your data into different periods. Rerun the notebook with the updated parameters To show this work, record the results in your `README.md` file. (4 points)

* Tune the trading algorithm by adjusting the SMA input features. Adjust one or both of the windows for the algorithm. Rerun the notebook with the updated parameters. To show this work, record the results in your `README.md` file. (4 points)

* Choose the set of parameters that best improved the trading algorithm returns. To show this work, save a PNG image of the cumulative product of the actual returns vs. the strategy returns, and document your conclusion in your `README.md` file. (2 points)

## Evaluate a New Machine Learning Classifier

In this section, you’ll use the original parameters that the starter code provided. But, you’ll apply them to the performance of a second machine learning model. To do so, complete the following steps:

1. Import a new classifier, such as `AdaBoost`, `DecisionTreeClassifier`, or `LogisticRegression`. (For the full list of classifiers, refer to the [Supervised learning page](https://scikit-learn.org/stable/supervised_learning.html) in the scikit-learn documentation.)

2. Using the original training data as the baseline model, fit another model with the new classifier.

3. Backtest the new model to evaluate its performance. Save a PNG image of the cumulative product of the actual returns vs. the strategy returns for this updated trading algorithm, and write your conclusions in your `README.md` file. Answer the following questions: Did this new model perform better or worse than the provided baseline model? Did this new model perform better or worse than your tuned trading algorithm?

## Summary