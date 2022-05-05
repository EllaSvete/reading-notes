# Class 13

## Code Challenge

- Use a Queue

## Lab

- choose a dataset
- make sure it has a csv
- questions about dataset

``` {python}
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

X = salary_df['YearsExperience'].values
X


y = salary_df['Salary'].values
y
//this gives an array of the salaries

plt.scatter(X, y)
// plots the data


//predictions
// plot the line based on the set of data

print(LinearRegression)
// checks sklearn is imported correctly, will show you the path

// in order to "fit" the model, need to adjust the shape of the data

year_experience_vector = X.reshape(-1, 1)
year_experience_vector

// creates 2d row of data
// reshapes the data for years

model = LinearRegression().fit(years_experience_vector, y)
model

// this returns our model and NOW we can make predictions


predictions = model.predict(years_experience_vector)
predictions

plt.scatter(X, y)
plt.plot(X, predictions, color="red")
plt.show()

num_years = 20
salary_predict = model.predict([ [num_years] ])
salary_predict

// this returns the prediction for a salary with  20 years of experience


// training the model

x_train, x_test, y_train, y_test = train_test_split(years_Experience_vector, salary_values, train_size = .8, test_size=.2)
x_test

```
