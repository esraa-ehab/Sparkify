# Sparkify

# Table of Contents
* [Installation](docs/Installation.md)
* [Project Motivation](docs/Project_Motivation.md)
* [Files Description](docs/Files_Description.md)
* [Results](docs/Results.md)
* [Licensing, Authors, and Acknowledgements](docs/Licensing,_Authors,_and_Acknowledgements.md)
# Installation
1. Install [pyspark](./http://spark.apache.org/downloads.html../) (I used [conda](./https://anaconda.org/conda-forge/pyspark../) to install it)

2. Install Java8 on your mac link

3. Open a new terminal and verify that Java is available on your mac by using the command below:
```
java -version
```
If you are seeing the message No Java runtime present, requesting install., you would need to add the following export to your ~/.bash_profile
```
export JAVA_HOME=/Library/Internet\ Plug-Ins/JavaAppletPlugin.plugin/Contents/Home
```
4. Start a jupyter notebook in a brand new terminal to use the new environment setting
# Project Motivation
For this project, I was interestested gaining experience with using Spark to

* Perform the Exploratory Data Analysis (EDA) with large and realistic datasets.
* Perform the Machine Learning process with Spark including Feature Creation, Model Training, Hyperparameter Tuning.
More specifically, I was interested in learning how to use Spark to manipulate large and realistic datasets with Spark to engineer relevant features for predicting churn, and also use Spark MLlib to build machine learning models with large datasets which is far beyond what could be done with non-distributed technologies like scikit-learn.
# Files Description
The [Sparkify.ipynb](./https://github.com/esraa-ehab/Sparkify/blob/master/Sparkify.ipynb../) notebook contains all steps in this process and markdown cells were used to assist in walking through the thought process for individual steps.
# Results
1. There are noticable differences between a ratio of gender, average session time, and an average number of songs played within a single session when comparing users who are churned and remain in service where:

   - Men have a much higher ratio to be churned
   - The average session time of users who remain in service is higher (303 minutes vs 283 minutes)
   - The average number of song per session of users who remain in service is higher (75 songs/session vs 70 songs/session)
2. A model trained from the Gradient-boosted tree classifier has a much better performance that a model trained form the Logistic Regression where the best model trained from the Gradient-boosted tree classifier achieved over 99% of area under ROC curve and has an accuracy over 97% while the best model trained from the Logistic Regression achieved only 70% of area under ROC and has an accuracy around 83%
# Licensing, Authors, and Acknowledgements
This project is [LICENSE](./https://github.com/esraa-ehab/Sparkify/blob/master/LICENSE../)

To see more about this analysis, see the link to my [Medium](https://medium.com/@esraa.ehab37/sparkify-7fb04056c7a6) available
