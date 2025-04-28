# Fraud Detection System

This project implements a fraud detection system to identify unusual (potentially fraudulent) purchase transactions. It uses machine learning models such as Decision Tree, Logistic Regression, and Naive Bayes, with hyperparameter tuning and evaluation metrics to determine the best-performing model.

## Folder Structure

```
Assignment_4/
├── data/                # Contains the dataset (e.g., Online_transaction_data.csv)
├── src/                 # Contains the source code (e.g., Assignment4.ipynb)
├── output/              # Contains the model predictions and results
└── README.md            # Instructions to run the solution
```

## Prerequisites

1. Python 3.7 or higher
2. Required Python libraries:
   - pandas
   - numpy
   - matplotlib
   - seaborn
   - scikit-learn

You can install the required libraries using the following command:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## How to Run

1. **Prepare the Dataset**  
   Place the dataset file (`Online_transaction_data.csv`) in the `data/` folder.

3. **Run the Jupyter Notebook**  
   Open the `src/Assignment4.ipynb` file in Jupyter Notebook or Jupyter Lab and execute the cells step by step.

   Alternatively, you can convert the notebook to a Python script and run it:

   ```bash
   jupyter nbconvert --to script src/Assignment4.ipynb
   python src/Assignment4.py
   ```

4. **View the Outputs**  
   The predictions and evaluation metrics for each model will be saved in the `output/` folder:
   - `decision_tree_predictions.csv`
   - `logistic_regression_predictions.csv`
   - `naive_bayes_predictions.csv`

5. **Evaluate the Results**  
   The notebook includes detailed evaluation metrics (precision, recall, F1-score) and confusion matrices for each model. Based on the results:
   - Decision Tree is recommended as the best-performing model.

## Key Features

- **Data Preprocessing**: Handles missing values, encodes categorical data, and scales features.
- **Feature Selection**: Uses Mutual Information and Random Forest to select the most important features.
- **Model Training**: Trains Decision Tree, Logistic Regression, and Naive Bayes models with hyperparameter tuning using GridSearchCV.
- **Evaluation**: Compares models using precision, recall, F1-score, and confusion matrices.

## Notes

- The dataset is highly imbalanced, so metrics like precision, recall, and F1-score are prioritized over accuracy.
- The Decision Tree model achieved the best balance between precision and recall, making it the most suitable for production deployment.

## Ethical Considerations

- **Bias Mitigation**: Care was taken to ensure the model does not introduce bias in predictions.
- **Privacy**: Encoded data ensures customer privacy is preserved.

## Contact

For any questions or issues, please contact [Your Name/Email].