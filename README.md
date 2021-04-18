Build a demand forecasting model to predict daily liquor sales in Iowa in 2021
==============================

Motivation
------------
Being a liquor retailer with retail stores across various locations in Iowa, the ability to accurately forecast daily demand for liquor consumption is key to avoid stockouts (which reduce customer satisfaction and result in revenue loss) as well as overstock (which causes higher than expected inventory and warehousing costs). Good demand forecasts reduce uncertainty as demand is extremely volatile and subjected to many influencing factors. 

However, traditional forecasting models such as ARIMA, AutoRegressive Integrated Moving Average, and exponential smoothing methods, where only historical data is considered, are getting outdated because of the increased amount of data generated from businesses and external sources.

Machine learning carries demand forecasting to the next step; it enables enhanced forecasts based on real-time data using internal and external data sources such as demographics, weather, online reviews and social media. With the help of external data and modern machine learning algorithms, supply chain networks can outperform networks managed more manually by data analysts and adapt to external changes. According to McKinsey Digital, ML-powered forecasting can reduces errors by 30 to 50% in supply chain networks. The improved accuracy leads up to a 65% reduction in lost sales due to inventory out-of-stock situations and warehousing costs decrease around 10 to 40%. 

In retail distribution and store replenishment, the benefits of good forecasting include the ability to attain excellent product availability with reduced safety stocks, minimized waste, as well as better margins, as the need for clearance sales are reduced. Further up the supply chain, good forecasting allows manufacturers to secure availability of relevant raw and packaging materials and operate their production with lower capacity, time and inventory buffers.

Owing to the potential business benefits, it makes sense to explore whether it is feasible to build an ML model to predict daily liquor demand in Iowa in 2021. 

Business Goals & Success Metrics
------------
I want to build a machine learning solution that predicts daily demand for liquor in Iowa for the next 30 days, with 90% accuracy. 

Being a liquor retailer with retail stores across various locations in Iowa, such a demand forecasting model can help me to better manage my inventory to ensure uninterrupted supply of products as well as avoid overstocking. 

To measure the forecast accuracy, applicable metrics include Mean Absolute Percentage Error (MAPE), Mean Absolute Error (MAE), Mean Absolute Deviation (MAD) and [forecast bias](https://www.relexsolutions.com/resources/measuring-forecast-accuracy/). It is important to note that forecast bias measures accuracy whereas MAD & MAPE measure forecast error. 


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
