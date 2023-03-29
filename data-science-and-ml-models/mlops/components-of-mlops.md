# Components of MLOps

Feature Store - Storing functions used in training the ML model. The functions are versioned, so that someone could revert to an older version if the latest features and functions aren't working

Data Versioning - Reproduction and facilitating audits

Metadata Store - It is essential to store information on all kind of data used. for eg. the seed used for splitting the train and validation set is not data that if present in the feature set but is important information when retraining or improving the model. Similarly the model metrics being used need to be consistent for different versions of the same model

Model Versioning - Allows you to switch between models in real time and also monitoring the metrics for different models.

Model Registration - Once a model has been trained, it is stored in a model registry with the metadata eg. neptune.ai, mlflow allows you to register your model to azure cloud. [https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-models?tabs=python%2Cuse-local#create-a-model-in-the-model-registry](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-models?tabs=python%2Cuse-local#create-a-model-in-the-model-registry)

Model serving - Creating endpoints that can be used to run predictions

Model monitoring - Checking deviation and bias that comes from change in data. Basically monitoring the statistics of train and validation, difference in performance of local and deployed models

Model retraining - Improve performance, availability of new data. Continuous Integration ensures that automated builds and test apply to change in data.

CI/CD - Frequent merge and deploy of model

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
