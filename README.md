# CSE151A_Project

**Feature information:**

Age: Age in years  
Ed: 1-Did not complete high school 2-High school degree 3-Some college degree 5-Prost-undergraduate degree  
Employ: Years with current employer  
Address: Years at current address  
Income: Household income in thousands  
Debtinc: Debt to income ratio (x100)  
Creddebt: Credit card debt in thousands  
Othdebt: Other debt in thousands  
Default: The "Default" field is the target variable, indicating previous defaulted. It takes binary values, with 1 typically denoting a "bad" default status and 0 representing a "good" repayment history.  

Summary: The Bankloan dataset was initially already relatively clean, with a select amount of NaN values that didn't heavily impact the dataset size which we subsequently dropped and cleaned. We also found an unrealistic outlier in the age column which we removed. We plotted our exploratory information on a pair plot, in which we gave distinct colors to defaulting being blue and vice versa. Furthermore, we made a heatmap to find statistical comparisons of the correlation of each column variable.

**Preprocessing:**
1. Removed an unrealistic outlier for age
2. Removed all rows with atleast one NaN
3. Standardized default column to be an 0 or 1
4. Generated pair plot for the dataset
5. Normalized dataset with MinMax scalar

## Model 1

Fitting Graph: Our model is outside the range of the ideal range and towards the underfitting section of the fitting graph

![grafik](https://github.com/austintnguyen/CSE151A_Project/assets/74422644/bf36c227-a93e-4252-b274-559cb981f009)

Next 2 expected models:

1. We would like to proceed to use a Deep Neural Network because we believe it would better identify complex patterns in the data that a basic logistic regression may not be able to. Specifically, since the logistic regression model seems to be underfitted, it would likely be improved by a Deep Neural Network. DNNs are also good at handling many features like we have in this dataset.
2.

Conclusion: Our model has a poor recall for predicting whether an individual defaults (does not pay off loan). The precision and recall for predicting whether an individual doesn't default (pays off loan) are 81% and 94% respectively. The testing MSE is relatively close to the training MSE but is slightly greater. Therefore, we believe our model is underfitted.
