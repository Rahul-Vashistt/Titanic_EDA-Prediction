# Titanic Survival Prediction

This project focuses on building a machine learning model to predict passenger survival on the Titanic using the classic Titanic dataset.

## Project Structure

```
├── data/
│   ├── train.csv
│   └── test.csv
├── EDA_titanic.ipynb
├── model_titanic.ipynb
├── requirements.txt
├── .gitignore
├── LICENSE (MIT)
└── README.md
```

## Notebooks

- **EDA_titanic.ipynb**  
  → Detailed Exploratory Data Analysis (EDA) on the Titanic dataset (currently a placeholder).

- **model_titanic.ipynb**  
  → Building the machine learning pipeline, training the model, and evaluating performance.

## Project Workflow

1. **Initial Basic Cleaning**:  
   - Dropping irrelevant columns like `PassengerId`, `Name`, `Ticket`, and `Cabin`.

2. **Train-Test Split**:  
   - Using an 80-20 split on the training data.

3. **Preprocessing**:  
   - Numerical features: Missing value imputation (`median`) + scaling (`StandardScaler`).
   - Categorical features: Missing value imputation (`most frequent`) + encoding (`OneHotEncoder`).
   - Managed using `ColumnTransformer` and `Pipeline`.

4. **Model Training**:  
   - Random Forest Classifier (100 trees, random_state=42).
   - Pipeline approach for clean and reproducible code.

5. **Evaluation**:  
   - Model accuracy on validation set: **~82.68%**.
   - Feature importance analysis.

## Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-link>
   cd <your-repo-folder>
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Dataset

The Titanic dataset (`train.csv` and `test.csv`) is available in the `/data/` folder.  
Original dataset source: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)

## License

This project is licensed under the MIT License.