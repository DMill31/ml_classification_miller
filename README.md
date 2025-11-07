# ml_classification_miller
# Miller Classification Midterm

## Project Overview
This project focuses on successfully creating a ML classification model on the UCI Mushroom dataset that can predict if a mushroom is poisonous or not

## Links

[This Notebook](https://github.com/DMill31/ml_classification_miller/blob/main/ml_midterm_miller.ipynb)

[Peer Review](https://github.com/DMill31/ml_classification_miller/blob/main/peer_review.md)

---
## Steps

### 1. Import and Inspect the Data

### 1.1 Import the necessary libraries
Numerous python libraries were needed, including pandas, seaborn, sklearn.  The dataset is also loaded and the first few rows are displayed.

### 1.2 Check for Missing Values and Display Summary Statistics
Every new dataset should be checked, so here the .info() and .describe() methods are utilized.  The UCI Mushroom dataset has '?' every instance there is a missing value, so that had to be taken into account to sum up missing values.

### 2. Data Exploration and Preparation

### 2.1 Explore Data Patterns and Distributions
Visuals are created to find any patterns in the data that can help lead us into knowing what input features to use.  Countplots and histograms are created because the dataset has exclusively categorical data.

### 2.2 Handle Missing Values and Clean Data
Here we drop a few useless features and rename the target variable for ease of understanding.

### 2.3 Feature Engineering
Categorical data is converted to numeric.  The feature 'habitat' has a few data types that rarely occur, so we sum those up into an 'other' group.  A few new features were made.  Lastly, all the features were encoded to be more model-friendly.

### 3. Feature Selection and Justification

### 3.1 Feature Selection
Due to the visuals created in section 2.1, the features chosen are:
- input features: odor & spore-print-color
- target feature: poisonous

### 3.2 Define X and y
Here we created the X and y variables that will be used in training/testing the models.

### 4. Train a Model (Decision Tree)

### 4.1 Split the data
We split the dataset into training and test sets using train_test_split().

### 4.2 Train the Model
In this section, the tree model is created and using the .fit() method it is trained.

### 4.3 Evaluate Performance
Now that the decision tree is trained, we can see how well it fares, so we make predictions and get the classification report.  A confusion matrix is made and the Decision Tree itself is also plotted for more visuals into this model.

### 5. Try Alternate Model

### 5.1 Train an Alternative Classifier (Logistic Regression)
Now instead of a decision tree, logistic regression will be used.  The model is created and trained using the same training data that the decision tree used.
Predictions are made, and again we print the classification report and a confusion matrix.

### 5.2 Compare Model Performances
A summary table is created to show the performance metrics of both the decision tree and logistic regression.

### 6. Final Thoughts and Insights

### 6.1 Summarize Findings
We find that the decision tree performed significantly better than the logistic regression, most likely due to the dataset being exclusively categorical and logistic regression always assuming linear separability.

### 6.2 Challenges Faced
A discussion of the troubles that came with this project is had.  They mostly revolve around still being new in terms of datasets with a large number of features and exclusively categorical data.  

### 6.3 What Would I Do Next?
If given more time, this project would go further by exploring the features that still remain untouched, as well as trying out different classifier models.

---
## How to Run the Project

### 1. Open the Notebook
This project's notebook can be found at:

ml_midterm_miller.ipynb

[notebook](https://github.com/DMill31/ml_classification_miller/blob/main/ml_midterm_miller.ipynb)

### 2. Activate the Virtual Environment & Select Kernel
In the terminal, run:

```shell
.\.venv\Scripts\activate
```

Once the virtual environment is up, at the top of the notebook select the kernel that goes with it

### 3. Run the Notebook
Either select the 'Run All' button at the top of the notebook or run the notebook cell by cell