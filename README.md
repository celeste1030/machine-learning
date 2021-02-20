# machine-learning-challenge
# Exoplanet Exploration

![K2-288Bb](Images/k2-288bb.jpg)

Created by [Celeste Muniz - Lithgow](https://github.com/celeste1030)

## Table of Contents
* [About](#about)
* [Source](#source)
* [Preprocessing the Data](#preprocessing-the-data)
* [Fit and Tune Model Parameters](#fit-and-tune-model-parameters)
* [Compare Models](#compare-models)
* [Technologies](#technologies)

## About

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I created machine learning models capable of classifying candidate exoplanets from the raw dataset.

## Source

[Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

## Preprocessing the Data
### EDA (Exploratory Data Analysis)
To explore the dataset and decide what to keep, I used visuals to observe properties of all of the columns in the dataframe.

### Seaborn Heat map

![heatmap1](Images/heatmap1.png)

I chose to use a Seaborn heat map to explore the data because it's useful way to see which columns are similar to each other. Columns that appear darker blue show that they are closely correlated to the column its paired with.  Columns that are too similar to each other may need to be deleted.  Many of these columns are margin of error columns.

### Histogram

![histogram army](Images/Xhist.png)

I explored the frequency of my X data by creating an army of histograms with pandas.  These histograms show me the frequency of attributes in each column which helps me narrow down what to keep for my model.  The more evenly distributed an attribute is, the more likely I am to keep it.

![histogram why](Images/yhist.png)

I also made a histogram for my y values.  This was useful to reference towards the end to see which y value needed to have the highest precision.  Later when I [compare models](#compare-models), "false positive" does have the highest precision showing that our model is useful for predicting the most recent y value.


* Perform feature selection and remove unnecessary features.
* Use an appropriate scaler to scale the numerical data.
* Separate the data into training and testing data.

## Fit and Tune Model Parameters
* Train and Test at least two models.
* Use `GridSearch` for at least one model to tune model hyperparameters.

## Compare Models
* Use evaluation metrics to compare models.
* Save the best model.

## Technologies

* Scikit-Learn
* Python
* Jupyter Notebook