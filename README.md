# Smoke Detection

This project uses environmental and air-quality sensor data to detect whether a fire alarm condition is present. The notebook in this repository analyzes sensor readings such as temperature, humidity, pressure, particulate matter, TVOC, and CO2-related values, then uses machine learning models to classify whether the system should trigger a fire alarm.

## Project Goal

The main objective is to build a classification model that predicts the target label `Fire Alarm` using IoT sensor data. The workflow includes:

- loading and inspecting the dataset
- performing exploratory data analysis (EDA)
- checking for missing or inconsistent values
- training and comparing classification models
- evaluating model performance

## Dataset

The project uses a sensor dataset from Kaggle that contains environmental measurements collected over time. The key features include:

- `UTC`
- `Temperature[C]`
- `Humidity[%]`
- `TVOC[ppb]`
- `eCO2[ppm]`
- `Raw H2`
- `Raw Ethanol`
- `Pressure[hPa]`
- `PM1.0`
- `PM2.5`
- `NC0.5`
- `NC1.0`
- `NC2.5`
- `CNT`
- `Fire Alarm` (target variable)

The target column is binary:

- `0` = no fire alarm
- `1` = fire alarm

## Repository Contents

- `Project_Code.ipynb` — the complete notebook with data loading, EDA, preprocessing, model training, and evaluation
- `README.md` — project overview and usage guide

## Tools and Libraries

This project is implemented using Python and the following libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `Jupyter Notebook`

## Setup

### Prerequisites

- Python 3.x
- Jupyter Notebook or Google Colab

### Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Run the Notebook

1. Open `Project_Code.ipynb` in Jupyter Notebook or Google Colab.
2. Ensure the dataset is accessible from the notebook.
3. Run all cells in order.

> Note: The notebook references a Google Drive-hosted CSV file. If you are running it outside the original environment, update the dataset path or download the CSV locally before executing the notebook.

## Workflow Summary

1. Import required Python libraries
2. Load the sensor dataset
3. Inspect the data structure and statistics
4. Check for missing values and feature distributions
5. Train classification models such as Random Forest and K-Nearest Neighbors
6. Evaluate model results and compare performance

## Project Use Case

This project is relevant to IoT-based safety and environmental monitoring systems, where early detection of hazardous conditions can help trigger alarms before a fire becomes critical.

## Notes

The notebook is designed as a practical data science and machine learning project focused on smoke/fire detection using sensor-based readings. It demonstrates how a real-world sensor dataset can be analyzed and used to build a predictive alarm system.
