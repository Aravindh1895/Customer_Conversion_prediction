# Customer_Conversion_prediction
# Insurance company- Customer Prediction Model

This repository contains a predictive model for an insurance organization to determine whether customers are likely to buy a product or not. The model has been trained and evaluated using various machine learning algorithms, including logistic regression, k-nearest neighbors (KNN), decision tree, random forest, and XGBoost. Among these algorithms, the XGBoost model demonstrated the highest performance based on AUROC score and F1 score.

## Dataset
The dataset consist of 45211 customer datas with 11 distinct features
The dataset used for training and evaluation consists of the following features:

- Age: Age of the person
- Job: Type of job
- Marital: Marital status
- Educational_qual: Education status
- Call_type: Contact communication type
- Day: Last contact day of the month (numeric)
- Mon: Last contact month of the year
- Dur: Last contact duration in seconds (numeric)
- Num_calls: Number of contacts performed during this campaign and for this client
- Prev_outcome: Outcome of the previous marketing campaign

## Target variable:
- y : has the client bought the product or not? denoted by yes or no

## Nature of the dataset:
The dataset is imbalanced, and to address this issue, the SMOTE-NN (Synthetic Minority Over-sampling Technique for Nominal and Numeric) method was used to balance the dataset.

## Model Fitting

After preparing the dataset and balancing it using SMOTE-NN, the XGBoost algorithm was selected as the final model due to its superior performance. The model was fitted using the preprocessed and balanced dataset to learn patterns and make predictions on new data.

## Evaluation Metrics

To assess the model's performance, the following evaluation metrics were considered:

- AUROC (Area Under the Receiver Operating Characteristic curve): Used to measure the model's ability to distinguish between positive and negative classes.
- F1 score: Represents the balance between precision and recall.

The XGBoost model achieved the highest AUROC score and F1 score, indicating its effectiveness in predicting customer behavior.

## Repository Structure

- `data/`: Contains the dataset used for training and evaluation.
- `notebooks/`: Google colab demonstrating the data preprocessing, model training, and evaluation steps.
- `models/`: Saved model files and related artifacts.
- `src/`: Source code for data preprocessing, model fitting, and evaluation.
- `README.md`: This file, providing an overview of the repository.

## Usage

To use the model, follow these steps:

1. Clone the repository: `https://github.com/Aravindh1895/Customer_Conversion_prediction.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Preprocess your own dataset or use the provided dataset in the `data/` directory.
4. Run the Google colab notebook for data preprocessing, model training, and evaluation.
5. Use the trained XGBoost model to make predictions on new data by calling appropriate functions in the source code within the `src/` directory.

Please refer to the individual notebooks and source code files for more detailed instructions.

## License

This project is licensed under the GPL License. You can find more information in the `LICENSE` file.

Feel free to contribute, raise issues, or submit pull requests if you have any improvements or suggestions for this project.


