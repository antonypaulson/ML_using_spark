# ML_using_spark
Machine learning using Scala on Apache Spark

## Description of Methodology

# Apache Spark: Model building

Using the `datasets/Heart.csv` dataset (credit: ISLR), build a binary classification model to predict whether or not the patient has heart disease (`AHD`) given the following features:

- `Age`
- `Sex`
- `ChestPain`
- `RestBP`
- `Chol`
- `Fbs`
- `RestECG`
- `MaxHR`
- `ExAng`
- `Oldpeak`
- `Slope`
- `Ca`
- `Thal`

## Data cleaning
1. Your target column (`AHD`) needs to be run through a `StringIndexer`.
2. `ChestPain` and `Thal` need to be run through a `StringIndexer` **and** a [`OneHotEncoderEstimator`](http://spark.apache.org/docs/latest/ml-features.html#onehotencoderestimator)


## Train/Test split
1. Split the data into an 80/20 train/test split. 
2. Best accuracy score from the test:

Logistic Regression: 0.8666666666666667
Random Forest Classifier: 0.822222

## Published Notebook:

https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/1005735361146337/391868758075581/6132986587663700/latest.html
