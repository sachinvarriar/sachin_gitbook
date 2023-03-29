# MLOps Stages

1. Model and Data version control
2. **AutoML** + Model and Data version Control
3. AutoML+ Model and Data Version Control + **Model Serving**
4. AutoML+ Model and Data Version Control + Model Serving + **Monitoring, Governance and Retraining**

**Data collection and Preparation -** developing features and feature storage are important eg. DVC, Feast

**Automated Development** - EDA > Feature Engineering > Training > Evaluation and testing

**Create ML Services** - Model needs to be integrated with enterprise application. The steps are

Event or request > API > Enrichement > Serve one or more models > Application response/Model and Data monitoring

**Monitoring, Governance and Retraining** - Automatic retraining based on a Ml model performance threshold
