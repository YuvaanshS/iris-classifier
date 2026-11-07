# Iris Flower Classifier

A beginner-friendly Jupyter notebook that walks through a complete supervised-learning workflow with scikit-learn, using the classic [Iris dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#iris-plants-dataset) (150 flowers, 3 species, 4 measurements each).

The dataset ships with scikit-learn, so there is nothing to download.

## What the notebook covers

1. **Explore the data**: summary statistics, class balance and a pairplot
2. **Train/test split**: 80/20, stratified so each species is represented evenly
3. **Train two models**: Logistic Regression (with feature scaling) and Random Forest
4. **Evaluate**: test accuracy, per-class precision/recall/F1 and confusion matrices
5. **Cross-validate**: 5-fold cross-validation for a more reliable estimate than a single split
6. **Interpret**: Random Forest feature importances
7. **Predict**: classify a new flower from its measurements

## Getting started

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# 2. (Optional) create a virtual environment
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Launch the notebook
jupyter notebook iris_classifier.ipynb
```

Then run the cells from top to bottom (**Kernel → Restart & Run All**).

## Project structure

```
.
├── iris_classifier.ipynb   # the notebook
├── requirements.txt        # Python dependencies
└── README.md
```

## Ideas for extending it

- Swap in another dataset, such as `load_digits()` (handwritten digits) or the Titanic data via `seaborn.load_dataset("titanic")`. Titanic needs missing-value handling and categorical encoding first.
- Tune hyperparameters with `GridSearchCV`.
- Try other models, such as `SVC`, `KNeighborsClassifier` or `GradientBoostingClassifier`.

## Tech stack

Python, scikit-learn, pandas, NumPy, matplotlib, seaborn, Jupyter
