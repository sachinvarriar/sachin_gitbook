# Bias and Variance in Machine Learning

### Errors in Machine Learning

In machine learning, an error is a measure of the accuracy of an algorithm/model to predict an unknown dataset. There are two type of error measures:

* **Reducible errors**: These errors can be reduced to improve the model accuracy. The two reducible errors we work on are bias and variance.
  * **Bias**:  The inability of a ML method to capture the true relationship. eg. Linear regression over a quadratic/polynomial relationship. The linear equation obtained has high bias.
  * **Variance**: The difference in fits between the train and test set is called as variance. In the above mentioned case of a linear regression fit over a otherwise possible quadratic equation, the linear equation has low variance.
* **Irreducible errors**: These errors can not be eliminated and will always be present in the model

### Bias-Variance Tradeoff

When ever a model fits well on the training set and not so well on the test set, we refer to this as over-fitting i.e, when ever we chose a high variance model we might end up over-fitting

The ideal ML model will have low bias and low variance. This is done by using sophisticated models like regularization, boosting and bagging. However an extremely low bias and low variance is not practically possible.

The different kind of models that we may get are

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**Low Bias - Low Variance**: This is the best case, but not practical always

**Low Bias - High variance**: Model predictions are inconsistent. These models typically have more parameters/features and lead to over-fitting

**High bias - Low variance**: These models don't learn well from the train dataset or have very few parameters/features. This leads to under-fitting

**High bias- High Variance**: Inconsistent results and low accuracy.



### Identifying High variance and High Bias

**High variance**: When a model has low training error and high test error

**High Bias**: High training error and test error is similar to the training error



### Bias-Variance tradeoff

For an accurate prediction of the model, algorithms need a low variance and low bias. But this is not possible because bias and variance are related to each other:

* If we decrease the variance, it will increase the bias.
* If we decrease the bias, it will increase the variance.

As a result we need to find the sweet spot between variance and bias&#x20;

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
