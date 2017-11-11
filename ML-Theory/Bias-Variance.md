# Bias Variance Tradeoff

## Keywords:
Bias, Variance,  Generalisation, Maximum Likelihood Esimation(MLE), VC dimension , Probably approximately correct(PAC)


## Quick Notes:


In statistics and machine learning, the bias–variance tradeoff (or dilemma) is the problem of simultaneously minimizing two sources of error that prevent supervised learning algorithms from generalizing beyond their training set. One of the major problems in Supervised learning.

Bias - The bias is error from erroneous assumptions in the learning algorithm. High bias can cause an algorithm to miss the relevant relations between features and target outputs (underfitting).

Variance - The variance is error from sensitivity to small fluctuations in the training set. High variance can cause overfitting: modeling the random noise in the training data, rather than the intended outputs.

Underfitting = high bias.

Overfitting = high variance.

Intuition:
If the model is too simple, the solution is biased and does not fit the data.
If the model is too complex then it is very sensitive to small changes in the data.

The bias-variance decomposition (often referred to as the bias-variance tradeoff) is a frequentist analysis of the generalization capability of an estimator, i.e. a learning algorithm.


## Detailed Notes: 


Normally, as you increase the complexity of your model, you will see a reduction in error due to lower bias in the model. However, this only happens till a particular point. As you continue to make your model more complex, you end up over-fitting your model and hence your model will start suffering from high variance.

A champion model should maintain a balance between these two types of errors. This is known as the trade-off management of bias-variance errors. Ensemble learning is one way to execute this trade off analysis.

Why is this important in the current context? To understand what really goes behind an ensemble model, we need to first understand what causes error in the model. We will briefly introduce you to these errors and give an insight to each ensemble learner in this regards.

Bias error is useful to quantify how much on an average are the predicted values different from the actual value. A high bias error means we have a under-performing model which keeps on missing important trends.

Variance on the other side quantifies how are the prediction made on same observation different from each other. A high variance model will over-fit on your training population and perform badly on any observation beyond training. Following diagram will give you more clarity (Assume that red spot is the real value and blue dots are predictions) :


> High Bias, High Variance
High-variance learning methods may be able to represent their training set well, but are at risk of overfitting to noisy or unrepresentative training data.
In contrast, algorithms with high bias typically produce simpler models that don't tend to overfit, but may underfit their training data, failing to capture important regularities.

The bias–variance tradeoff is a central problem in supervised learning. Ideally, one wants to choose a model that both accurately captures the regularities in its training data, but also generalizes well to unseen data. Unfortunately, it is typically impossible to do both simultaneously.



> Generalisation 

When we fit a statistical model, we are interested in generalizing, i.e. making good predictions on data we haven't seen yet. We can fail at this in two ways: by underfitting (missing important structure in the data), or by overfitting (where the model is too sensitive to idiosyncrasies in the data).

We can measure the generalization error of a model by training it on a training set  and then evaluating it on a separate test set. Understanding the tradeoffs of model fit vs. complexity and how to measure generalization is key to getting any machine learning algorithm to work in practice.

Probably approximately correct (PAC) learning is a theoretical framework for analyzing the generalization error of a learning algorithm in terms of its error on a training set and some measure of complexity. The goal is typically to show that an algorithm achieves low generalization error with high probability.



The bias-variance decomposition (math)

Err(x) = Bias^2 + Variance + Irreducible Error

It means that every time we have error, it's either because of bias or because of variance.


## Advanced Resources/Reference:


https://www.coursera.org/learn/machine-learning/lecture/yCAup/diagnosing-bias-vs-variance

http://machinelearningmastery.com/gentle-introduction-to-the-bias-variance-trade-off-in-machine-learning/

http://scott.fortmann-roe.com/docs/BiasVariance.html

https://www.coursera.org/learn/machine-learning/lecture/4VDlf/regularization-and-bias-variance