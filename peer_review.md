# Peer Review

## Peer: Blessing Aganaga
## Notebook: [Link](https://github.com/teflxndxn/ml_classification_blessing/blob/main/classification_blessing.ipynb)

---

### 1. Clarity & Organization

**Strengths:**
Blessing's notebook follows a logical structure (Imports -> EDA -> Cleaning -> Modeling -> Evaluation -> Reflection), showing a clear workflow.  Adding markdown cells for small pieces of info here and there is also very helpful in understanding the notebook.  The reflections summarize everything well and are written without being overly academic.

**Growth Areas:**
The headings could use some work.  There are headings in the notebook that are different sizes and a few that use the same number.  For instance, both "2.2 Count unique values for categorical variables" and "2.2 Handle Missing Values" are present.

### 2. Feature Selection & Justification

**Features Chosen:**
Input features:
- Pclass
- Sex_male
- Age
- Fare
- Embarked_Q
- Embarked_S

Target:
- Survived

**Strengths:**
These features each make sense conceptually.  Fare and Pclass give insights into passenger class and wealth, which did have an affect on lifeboat access.  Age and Sex_male are very strong predictors as we found age to be quite strong in a previous project and we know historically that males did not have the best chance of survival given the "women and children first" policy they followed.  As for Embarked_S and Embarked_Q, we get some info about passenger demographics by region, which might have an indirect correlation with survival.  

**Growth Areas:**
There may be some redundancy to consider in the features chosen.  For instance, Pclass and Fare are highly correlated which should be kept in mind and acknowledged.  There was also no reflection 3 to tell readers why those specific features were chosen.  

### 3. Model Performance & Comparisons

**Strengths:**
Multiple evaluation metrics are given: accuracy, precision, ROC AUC, etc.  Not only that but the ROC and precision-recall curves are plotted, which makes understanding the results a lot easier.  Continuing with visuals, having the curves from the different models together in section 5.2 makes understanding the difference in model performance a lot better as we can compare the curves without having to scroll.

**Growth Areas:**
While classification reports and ROC AUC curves are plotted, a summary table at the end would be the bow on top to help the reader fully understand how the models compare.  

### 4. Reflection Quality

**Strengths:**
The reflections are well thought out and even real-world scenarios are discussed.  Enhancers like bold text and bullet points make the reflections easier to understand.  The summary at the end (reflection 6) is an exemplary reflection.  It's super easy to follow along with and successfully summarizes the most important part of the notebook.

**Growth Areas:**
As mentioned, reflection 3 is missing.  In terms of formatting, the reflections are either paragraphs or bullet point lists, I believe it would be best to stick with one format for the whole notebook.  