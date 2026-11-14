# Iris Flower Classification

An introductory machine learning project that explores the Iris dataset and trains a **support vector classifier** to distinguish three flower species from four measurements.

## Workflow
1. Load the local `iris.data` file with Pandas.
2. Explore class distributions visually with a Seaborn pair plot.
3. Compare average feature values by species.
4. Split the data into **80% training / 20% test**.
5. Train scikit-learn's `SVC` and print a classification report.
6. Predict species for three example measurements.

## Run locally
From the repository root:

```sh
python -m venv .venv
source .venv/bin/activate
pip install numpy pandas matplotlib seaborn scikit-learn
python IrisClassification.py
```

The script prints precision, recall and F1 scores for the test split, followed by example predictions. Figures are created in memory; saving/displaying them is commented out in the current script.

## Visual exploration
![Pairwise feature relationships](pairplot.png)
![Mean feature values by species](features_means.png)

## Evaluation limits
This is a learning baseline. The current split has no fixed random seed or stratification, and there is no cross-validation or feature-scaling pipeline. Results can vary between runs; no fixed accuracy is claimed here.

## Files
- [Training and exploration script](IrisClassification.py)
- [Dataset](iris.data)
- [Dataset description and source information](iris.names)

**Stack:** Python · Pandas · NumPy · scikit-learn · Seaborn · Matplotlib
