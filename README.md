# Titanic Survival Prediction

This project predicts the survival of passengers aboard the Titanic using machine learning techniques. The dataset is preprocessed and analyzed to train a Random Forest Classifier for prediction.

## Project Structure

- **`titanic_survival.ipynb`**: Jupyter Notebook containing the code for data preprocessing, analysis, and model training.
- **`.gitignore`**: Specifies files and directories to be ignored by Git.
- **`README.md`**: Documentation for the project.

## Dataset

The dataset used in this project is a CSV file named `titanic_analysis.csv`. It contains information about Titanic passengers, including their survival status, age, gender, class, and other features.

## Steps in the Notebook

1. **Environment Setup**:
   - Load environment variables using `dotenv`.
   - Read the dataset from the specified path.

2. **Data Preprocessing**:
   - Handle missing values in columns like `Age` and `Embarked`.
   - Drop unnecessary columns such as `Cabin`, `Ticket`, `Fare`, `Name`, and `Embarked`.
   - Convert categorical data (e.g., `Sex`) into numerical format.

3. **Exploratory Data Analysis**:
   - Analyze the dataset using methods like `.head()`, `.info()`, and `.describe()`.

4. **Feature Engineering**:
   - Prepare the dataset for machine learning by separating features (`X`) and target (`y`).

5. **Model Training**:
   - Split the dataset into training and testing sets.
   - Train a Random Forest Classifier on the training data.

6. **Model Evaluation**:
   - Predict survival on the test set.
   - Evaluate the model's accuracy using `accuracy_score`.

## Requirements

- Python 3.x
- Libraries:
  - `numpy`
  - `pandas`
  - `scikit-learn`
  - `python-dotenv`

## How to Run

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd titanic_survival_prediction
2.  Install dependencies:
    pip install -r requirements.txt
3. Create a .env file and specify the path to the dataset:
   DATASET_PATH=path/to/titanic_analysis.csv
4.  Open the Jupyter Notebook:
   jupyter notebook [titanic_survival.ipynb] 
    (http://_vscodecontentref_/1)
5.  Run the cells in the notebook to preprocess the data, train the 
    model, and evaluate its performance.

Results: 
The Random Forest Classifier achieves an accuracy of approximately 81% on the test set.