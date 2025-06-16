# FIFA Player Rating Prediction with Linear Regression
<div align="center">
  <img src="https://github.com/rahulkumargit1/FIFA-Player-Rating-Prediction-with-Linear-Regression/blob/main/dataset-cover.jpg" alt="fifa cover" style="width: 100%; max-width: 800px; height: auto; border-radius: 10px;">
</div>
## Project Overview
This project aims to predict player ratings in FIFA 23 using linear regression. The dataset, `FIFA23_official_data.csv`, contains detailed attributes of football players, including their age, nationality, club, overall rating, potential, value, wage, and various performance metrics. The analysis includes data preprocessing, exploratory data analysis, and building a linear regression model to predict the `Overall` rating based on selected features.

## Dataset
The dataset (`FIFA23_official_data.csv`) includes 29 columns, such as:
- **ID**: Unique player identifier
- **Name**: Player's name
- **Age**: Player's age
- **Nationality**: Player's country
- **Overall**: Player's overall rating (target variable)
- **Potential**: Player's potential rating
- **Club**: Player's current club
- **Value**: Player's market value
- **Wage**: Player's weekly wage
- **Preferred Foot**, **International Reputation**, **Weak Foot**, **Skill Moves**, **Work Rate**, **Body Type**, **Height**, **Weight**, **Release Clause**, **Kit Number**: Additional player attributes

The dataset contains some missing values (e.g., in `Loaned From` and `Best Overall Rating`) and URL-based columns (e.g., `Photo`, `Flag`, `Club Logo`).

## Requirements
To run the notebook, ensure the following Python libraries are installed:
```bash
pip install numpy pandas seaborn matplotlib eli5 missingno plotly
```

## Usage
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Prepare the Dataset**:
   - Place the `FIFA23_official_data.csv` file in an accessible directory.
   - Update the file path in the notebook to match your local environment (currently hardcoded to `E:\LIVEIMAGE\Machine Learning Project 12 - Hand Digit Recognition Using ML\FIFA23_official_data.csv`).

3. **Run the Notebook**:
   - Open `fifa-in-depth-analysis-with-linear-regression-checkpoint.ipynb` in Jupyter Notebook or JupyterLab.
   - Execute the cells to load the data, preprocess it, and visualize the results.

4. **Key Features**:
   - **Data Loading**: Uses `pandas` to load the CSV file.
   - **Visualization**: A regression plot (`seaborn.regplot`) shows predicted vs. actual player ratings.
   - **Feature Importance**: Uses `eli5` and `PermutationImportance` to analyze which attributes most influence the `Overall` rating.
   - **Missing Data**: Handled with the `missingno` library.

## Results
The project includes a visualization of the linear regression model's predictions, plotting predicted player ratings against actual ratings. The scatter plot uses red points with blue edges and a black regression line to illustrate model performance.

## Notes
- The notebook references variables (`predictions`, `y_test`) that are not defined in the provided code, indicating that model training and data splitting steps are implemented in earlier cells.
- The hardcoded dataset path may need to be updated for portability.
- The notebook contains empty cells, suggesting it is a checkpoint or work-in-progress.

## Future Improvements
- Include the model training and data preprocessing code in the notebook for completeness.
- Add cross-validation to evaluate the model's performance robustly.
- Handle missing values explicitly and document the approach.
- Explore additional machine learning models (e.g., Random Forest, XGBoost) for improved accuracy.

## Author
- **Rahul**

## License
This project is licensed under the MIT License.
