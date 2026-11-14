# predict_future_sales

<a target="_blank" href="https://cookiecutter-data-science.drivendata.org/">
    <img src="https://img.shields.io/badge/CCDS-Project%20template-328F97?logo=cookiecutter" />
</a>

Forecasting de ventas mensuales por tienda-producto (Predict Future Sales, Kaggle)

## Cómo empezar

1. Clonar el repositorio y actualizarlo:
   ```bash
   git clone <url-del-repositorio>
   cd <carpeta-del-repositorio>
   git pull
   ```
2. Crear el entorno conda (Python 3.11) e instalar las dependencias:
   ```bash
   conda create -n env_predict_future_sales -c conda-forge python=3.11 "libblas=*=*openblas"
   conda activate env_predict_future_sales
   pip install -r requirements.txt
   ```
3. Descargar los datos de [Kaggle](https://www.kaggle.com/competitions/competitive-data-science-predict-future-sales/data)
   y colocar los CSV en `data/raw/` (no se versionan). Otra carpeta se puede indicar con la variable de entorno `DATA_DIR`.
4. Abrir `notebooks/01_exploratory_data_analysis.ipynb` con el kernel `env_predict_future_sales`.

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         predict_future_sales and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── predict_future_sales   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes predict_future_sales a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------

