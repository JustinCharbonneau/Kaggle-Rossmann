Kaggle-Rossman
==============================

Explore XGBoost for Regression on Kaggle-Rossman and Entity Embeddings in PyTorch.


## Summary Results

Private score and puplic score were retreived after submitting the predictions to Kaggle.

| Experiment ID | Categorical Variables | NaN-cats | NaN-cont | Target Transformation | Hyperparameter Search | Backtesting            | Private Score | Public Score
|---------------|-----------------------|----------|----------|-----------------------|-----------------------|------------------------|---------------|---------------
| 001           | Target encoder        | XGBoost  | XGBoost  | Log transform         | Default               | No                     | 0.16925       | 0.17975
| 002           | Target encoder        | XGBoost  | XGBoost  | Log transform         | HyperOpt (100)        | TimeSeriesSplit k = 3  | 0.13975       | 0.12481
| 003           | Entity Embeddings     | #NAN#    | FastAI   | Log transform         | Default               | No                     | 0.15251       | 0.14079
| 004           | Entity Embeddings     | #NAN#    | FastAI   | Log transform         | HyperOpt (100)        | TimeSeriesSplit k = 3  | 0.13081       | 0.11572




Project Organization
------------

    ├── README.md          <- The top-level README for developers using this project.
    ├── data
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



--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
