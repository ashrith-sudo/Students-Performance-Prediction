# Students Performance Prediction

This project analyzes student performance data to predict math scores using machine learning. The workflow includes data loading, preprocessing, feature engineering, model selection, and interpretation of results. The core analysis is implemented in the Jupyter notebook [`Student_Performance.ipynb`](Student_Performance.ipynb).

## Dataset

- Source: `StudentsPerformance.csv`
- Features include:
  - **gender**
  - **race/ethnicity**
  - **parental level of education**
  - **lunch**
  - **test preparation course**
  - **math score**, **reading score**, **writing score**

## Workflow

### 1. Data Loading

- The dataset is loaded into a pandas DataFrame.
- The first five rows, column names, and data types are displayed to understand the structure and types of the data.

### 2. Data Preprocessing

- **Missing Values:** The dataset is checked for missing values in each column. No missing values are found, so no imputation is necessary.

### 3. Feature Engineering

- **Encoding Categorical Variables:** All categorical features are converted to numerical representation using one-hot encoding (via `pd.get_dummies`), making them suitable for machine learning models.

### 4. Model Preparation

- **Splitting Data:** The data is split into training and testing sets to evaluate model performance. (Details are in the notebook.)

### 5. Model Selection and Training

- Multiple regression models are explored to predict math scores based on the other features.
- Appropriate metrics are used to evaluate and compare model performance.

### 6. Feature Importance

- The models are interpreted to identify which features most strongly influence student math performance.
- Overfitting is addressed by comparing training and test performance and applying regularization or simpler models as needed.

## How to Run

1. Clone the repository.
2. Open `Student_Performance.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells in order. Make sure `StudentsPerformance.csv` is available at the correct path (or update the path as needed).

## Results

- The project identifies key factors influencing student math scores.
- A regression model is built that can predict a student's math score based on other observed characteristics.

## Repository Structure

- `Student_Performance.ipynb` – Main analysis notebook
- `StudentsPerformance.csv` – Dataset (not included in repo, see notebook for details)

## References

- The notebook is self-documented with reasoning and explanations for each step.
- See the notebook for code, outputs, and further interpretation.

---

**For more details, see the notebook:**  
[Student_Performance.ipynb](Student_Performance.ipynb)
