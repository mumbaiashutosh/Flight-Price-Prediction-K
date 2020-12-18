# Flight-Price-Prediction-K
Importing dataset
Since data is in form of excel file we have to use pandas read_excel to load the data
![Structure](https://user-images.githubusercontent.com/56570977/102611845-bd5dd180-4155-11eb-8745-8a4f0f2b4f14.JPG)

After loading it is important to check the complete information of data as it can indication many of the hidden infomation such as null values in a column or a row
Check whether any null values are there or not. if it is present then following can be done,
Imputing data using Imputation method in sklearn
Filling NaN values with mean, median and mode using fillna() method
Describe data --> which can give statistical analysis

EDA
From description we can see that Date_of_Journey is a object data type, Therefore, we have to convert this datatype into timestamp so as to use this column properly for prediction
For this we require pandas to_datetime to convert object data type to datetime dtype.
.dt.day method will extract only day of that date
.dt.month method will extract only month of that date

This project is important fromt the standpoint that there are many values which exist as categorical variables. We convert them one by one
So we get the required values in our desired types and drop those columns

So we do this for Arrival and Departure Date and Time as well as Duration. 
