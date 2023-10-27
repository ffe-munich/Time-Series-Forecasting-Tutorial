# Predictions in Energy Economics - Tutorial on Household and PV Load Forecasting
The energy industry is facing significant challenges that require high adaptability and the utilization of flexibility. To optimize the integration of renewable energies and harness the potential of electric mobility and heat pumps, reliable predictions are indispensable. In this series of articles, some fundamental concepts of machine learning have been introduced, such as [appropriate metrics for evaluating prediction quality](https://www.ffe.de/en/publications/predictions-in-energy-economics-which-error-metrics-are-suitable/), [various machine learning methods for time series forecasting](https://www.ffe.de/en/publications/predictions-in-energy-economics-which-methods-are-suitable/), and [their advantages and disadvantages](https://www.ffe.de/en/publications/predictions-in-energy-economics-which-methods-are-suitable/). This article provides a practical example of how to perform time series forecasting using a Jupyter notebook.

# Tutorial on Household and PV Load Forecasting

In the `time_series_forecasting.ipynb` you can find the tutorial. For this tutorial, [public data from the pilot operation of the BDL project](https://opendata.ffe.de/dataset/electric-load-profiles-and-vehicle-data-of-private-households-with-a-bidirectional-ev/), which records household and PV load from various buildings, is used. Initially, some features are extracted from the time series, which can be derived from temporal information or from past values or their statistical properties. Subsequently, the time series is divided into training and testing data, and the correlation of features in the training dataset is examined. Finally, linear regression and a Random Forest Regressor are applied to make predictions. Metrics for both models are also calculated and compared to assess their performance.

# Setup

1. Create a virtual envoirnment with the requirements (or install them to your local python version):
> `> virtualenv -p python3 venv`

> `> source venv/bin/activate`

> `> pip install requirements.txt`

2. The tutorial can be found in the notebook: `time_series_forecasting.ipynb`
