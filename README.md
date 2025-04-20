# ml_regression_drake
Final Project: Regression Analysis
Submission: GitHub Repository with Jupyter Notebook and Peer Review

Overview
Businesses and organizations often need to understand the relationships between different factors to make better decisions. For example, a company may want to predict the fuel efficiency of a car based on its weight and engine size or estimate home prices based on square footage and location. Regression analysis helps identify and quantify these relationships between numerical features, providing insights that can be used for forecasting and decision-making.

This project demonstrates your ability to apply regression modeling techniques to a real-world dataset. You will:

Load and explore a dataset.
Choose and justify features for predicting a target variable.
Train a regression model and evaluate performance.
Compare multiple regression approaches.
Document your work in a structured Jupyter Notebook.
Conduct a peer review of a classmate's project.
Dataset Options
Select one dataset from the list below. If you get good results, you can try the process on a suitable dataset of your own. Suitable datasets contain numerical features and a numerical target variable for regression.

Auto MPG Dataset (Predict fuel efficiency based on engine specs and weight)
UCI Auto MPG Dataset
Housing Prices Dataset (Predict home values based on features like square footage and location)
Kaggle Housing Prices
Medical Costs Dataset (Predict insurance charges based on age, BMI, smoking status)
Medical Cost Dataset
Assignment Requirements
Your Jupyter Notebook must follow a structured format with clearly numbered second-level headings and reflection remarks after each section.

Create a virtual environment:
# Create your local project virtual environment
# This step ensures you have an isolated Python environment for your project.
# This is typically just done once at the beginning of a project.
# If it gets messed up, we can delete .venv and recreate it at any time. 

# Run the following command to create a virtual environment in the project root.
### On Windows, Use PowerShell (not cmd) - don't include the #:
# py -m venv .venv

Activate the virtual environment: 
# ALWAYS activate the .venv before working on the project.
# Activate whenever you open a new terminal. 

### Windows PowerShell Command (don't include the #):
# .venv\Scripts\activate

# Install necessary packages listed below with this command:
# Keep packages updated with the most recent versions.

# When you identify a new package you want to use, 
# Just update the list below and re-run this command. 

### Windows Command (don't include the #):
# py -m pip install --upgrade pip setuptools wheel
# py -m pip install -r requirements.txt

Start your notebook professionally with:

a single top-level title
your name (or alias)
the date
a brief introduction that describes the problem and the dataset.
Import the external Python libraries used (e.g., pandas, numpy, matplotlib, seaborn, sklearn).
Section 1. Import and Inspect the Data
1.1 Load the dataset and display the first 10 rows.
1.2 Check for missing values and display summary statistics.
Reflection 1: What do you notice about the dataset? Are there any data issues?

Section 2. Data Exploration and Preparation
2.1 Explore data patterns and distributions
Create histograms, boxplots, and count plots for categorical variables (as applicable).
Identify patterns, outliers, and anomalies in feature distributions.
Check for class imbalance in the target variable (as applicable).
2.2 Handle missing values and clean data
Impute or drop missing values (as applicable).
Remove or transform outliers (as applicable).
Convert categorical data to numerical format using encoding (as applicable).
2.3 Feature selection and engineering
Create new features (as applicable).
Transform or combine existing features to improve model performance (as applicable).
Scale or normalize data (as applicable).
Reflection 2: What patterns or anomalies do you see? Do any features stand out? What preprocessing steps were necessary to clean and improve the data? Did you create or modify any features to improve performance?

Section 3. Feature Selection and Justification
3.1 Choose features and target
Select two or more input features (numerical for regression, numerical and/or categorical for classification)
Select a target variable (as applicable)
Regression: Continuous target variable (e.g., price, temperature).
Classification: Categorical target variable (e.g., gender, species).
Clustering: No target variable.
Justify your selection with reasoning.
3.2 Define X and y
Assign input features to X
Assign target variable to y (as applicable)
Reflection 3: Why did you choose these features? How might they impact predictions or accuracy?

Section 4. Train a Model (Linear Regression)
4.1 Split the data into training and test sets using train_test_split (or StratifiedShuffleSplit if class imbalance is an issue).
4.2 Train model using Scikit-Learn model.fit() method
4.3 Evalulate performance, for example:
Regression: R^2, MAE, RMSE (RMSE has been recently updated)
Classification: Accuracy, Precision, Recall, F1-score, Confusion Matrix
Clustering: Inertia, Silhouette Score
Reflection 4: How well did the model perform? Any surprises in the results?

Section 5. Improve the Model or Try Alternates (Implement Pipelines)
5.1 Implement Pipeline 1: Imputer → StandardScaler → Linear Regression.
5.2 Implement Pipeline 2: Imputer → Polynomial Features (degree=3) → StandardScaler → Linear Regression.
5.3 Compare performance of all models across the same performance metrics
Reflection 5: Which models performed better? How does scaling impact results?

Section 6. Final Thoughts & Insights
6.1 Summarize findings.
6.2 Discuss challenges faced.
6.3 If you had more time, what would you try next?
Reflection 6: What did you learn from this project?

Tasks to Complete the Assignment
Create a GitHub repository named ml_regression_yourname.
Upload your dataset to a data folder in the repository.
Develop a Jupyter Notebook (regression_yourname.ipynb) structured as outlined above.
Complete and write reflections for each section as you work.
Write a README.md summarizing your project, dataset, and findings (see below).
Review a classmate’s project and provide feedback in peer_review.md (see below).
README.md (Required)
Include a professional README.md that introduces your project. Include:

a clickable link to your notebook file.
a clickable link to your your peer review Markdown file.
Instructions on how to set up your virtual environment and run your notebook locally.
Peer Review (Required)
Review one other GitHub repository and provide feedback on:

Clarity & Organization (Is the notebook structured and easy to follow?)
Feature Selection & Justification (Do the chosen features make sense given the objectives?)
Model Performance & Comparisons (Are the results and comparisons clearly explained?)
Reflection Quality (Are insights well thought out?)
Submission: Submit a short peer review document in your own repository titled peer_review.md.
The peer review must contain a clickable Markdown link to the notebook (.ipynb) file reviewed along with your personal, well-organized and presented 4-pont review. Provide specifics - both positive and constructive feedback. Suggest improvements where possible and explain why a different choice might be useful as well. Focus on actionable suggestions that the author could realistically implement.

4-point Repository Checklist
Verify your repository contains:

[ ] Jupyter Notebook with proper name, numbered sections and reflections.
[ ] README.md (see above) [ ] Dataset, stored in a data folder.
[ ] Peer Review (peer_review.md).

