# Cross Validation with Linear Regression

This project demonstrates the use of cross-validation to evaluate the performance of a linear regression model using CGPA and salary package data. The objective is to predict the salary package based on a student's CGPA using k-fold cross-validation for better model assessment.

## Dataset

The dataset contains the following columns:
- `CGPA`: Cumulative Grade Point Average of students.
- `Package (in LPA)`: Salary package offered to the students (in Lakhs Per Annum).

Sample data:
| CGPA | Package (in LPA) |
|------|------------------|
| 2.1  | 3.0              |
| 2.5  | 4.0              |
| 2.8  | 5.0              |
| 3.0  | 6.0              |
| 3.2  | 7.0              |

## Libraries Used

The following Python libraries are used in this project:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `sklearn`

## Project Workflow

1. **Loading the Dataset**: The dataset is read using `pandas`.
2. **Data Visualization**: A scatter plot is created using `seaborn` to visualize the relationship between CGPA and the offered salary package.
3. **Model Definition**: A Linear Regression model is created using the `LinearRegression()` function from `sklearn`.
4. **Cross Validation**: Cross-validation is implemented using `cross_val_score` and KFold for more accurate evaluation of the model.

### Example Scatter Plot
```python
sns.scatterplot(x="CGPA", y="Package (in LPA)", data=dataset)
plt.show()
