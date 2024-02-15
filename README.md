# CSE151A_Project

**Preprocessing Information**:

Column information:

Age: Age in years  
Ed: 1-Did not complete high school 2-High school degree 3-Some college degree 5-Prost-undergraduate degree  
Employ: Years with current employer  
Address: Years at current address  
Income: Household income in thousands  
Debtinc: Debt to income ratio (x100)  
Creddebt: Credit card debt in thousands  
Othdebt: Other debt in thousands  
Default: The "Default" field is the target variable, indicating previous defaulted. It takes binary values, with 1 typically denoting a "bad" default status and 0 representing a "good" repayment history.  

The Bankloan dataset was initially already relatively clean, with a select amount of NaN values that didn't heavily impact the dataset size which we subsequently dropped and cleaned. We also found an unrealistic outlier in the age column which we removed. We plotted our exploratory information on a pair plot, in which we gave distinct colors to defaulting being blue and vice versa. Furthermore, we made a heatmap to find statistical comparisons of the correlation of each column variable.

Preprocessing:
1. Removed an unrealistic outlier for age
2. Removed all rows with atleast one NaN
3. Standardized default column to be an 0 or 1
4. Generated pair plot for the dataset
5. Normalized dataset with MinMax scalar

**Model 1**

