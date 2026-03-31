# Water Quality Analysis and Prediction

This project analyzes water quality data and builds machine learning models to predict whether a water sample meets quality standards.

## Project Overview

The notebook `water_quality_analysis_solution.ipynb` explores a large water quality dataset, performs data cleaning and preprocessing, conducts exploratory data analysis (EDA), engineers features, trains classification models, and interprets the most important factors affecting water quality.

## Dataset

The main dataset is expected in the `data/` folder as:
- `data/water_quality_dataset_100k_new.csv`

### Data Description

The dataset contains water quality measurements from various water sources, including:
- pH, Iron, Nitrate, Chloride, Lead, Zinc, Fluoride, Copper, Manganese, Sulfate, Chlorine
- Color, Odor, Turbidity, Conductivity, Total Dissolved Solids (TDS)
- Water Temperature, Air Temperature, sampling Month, Day, and Time of Day

The binary target variable `Target` indicates whether the sample meets water quality standards.

The notebook also references the original dataset sources:
- Subset dataset: https://drive.google.com/file/d/1NPnyvMMa4EgRMpCWd1LOOVGeOOmtcC6f/view?usp=drive_link
- Original dataset on Kaggle: https://www.kaggle.com/datasets/mitanshuchakrawarty/water-quality-prediction/data?select=dataset.csv

## Key Steps

1. Data loading and inspection
2. Missing value handling and imputation
3. Categorical encoding and numerical scaling
4. Exploratory Data Analysis (histograms, box plots, scatter plots, correlation heatmaps)
5. Feature engineering and new feature creation
6. Train/test split and model training
7. Model evaluation with accuracy, precision, recall, and F1-score
8. Model interpretation and feature importance analysis

## Models Compared

The notebook trains and evaluates several models including:
- Logistic Regression
- Random Forest
- K-Nearest Neighbors
- Decision Tree

The best model is selected based on evaluation metrics and then interpreted to reveal the most influential water quality factors.

## Important Files

- `water_quality_analysis_solution.ipynb` - main analysis and modeling notebook
- `data/water_quality_dataset_100k_new.csv` - dataset used for the analysis
- `data/preprocessed.csv` - preprocessed dataset output from the notebook

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tqdm
- xgboost

## How to Run

1. Open `water_quality_analysis_solution.ipynb` in Jupyter Notebook or VS Code.
2. Make sure the data file is available at `data/water_quality_dataset_100k_new.csv`.
3. Install the required Python packages if needed.
4. Run the notebook cells in order.

## Notes

- The notebook uses `MinMaxScaler` for normalization and `OneHotEncoder` for categorical encoding.
- The analysis includes both visualization and model performance comparison.
- The final section includes recommendations for improving water quality based on model findings.

## License

This project is provided for educational and portfolio use. Feel free to adapt it for your own analysis.
