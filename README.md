# CodSoft
This is my repository for CodSoft Internship
--------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------
1st Project -> Credit Card fraud Detection using Classification Algorithms such as Random Forest and Decision Tree
--------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------
Reading the train and test CSV file
--------------------------------------------------------------------------------------------------------------------
Training -> head
--------------------------------------------------------------------------------------------------------------------
create a pie graph 
--------------------------------------------------------------------------------------------------------------------
Count the value of is fraud -> 1 and is not fraud -> 0
--------------------------------------------------------------------------------------------------------------------
Yellow colour represents Genuine and Black colour represents Fraud
--------------------------------------------------------------------------------------------------------------------
In this code snippet results we can see that we have very low amount of people
--------------------------------------------------------------------------------------------------------------------
We have very low frauds
--------------------------------------------------------------------------------------------------------------------
In this code we have Genuine -> we count num of zeros and then find percentage
--------------------------------------------------------------------------------------------------------------------
In this code we have Fraud -> we count num of ones and then find percentage
--------------------------------------------------------------------------------------------------------------------
Give us the information of training dataframe
--------------------------------------------------------------------------------------------------------------------
Give us the information of testing dataframe
--------------------------------------------------------------------------------------------------------------------
Now we are removing null values from train dataframe
--------------------------------------------------------------------------------------------------------------------
Now we are removing null values from test dataframe
--------------------------------------------------------------------------------------------------------------------
Drop Columns that are not relevant to predicy fraud transaction
--------------------------------------------------------------------------------------------------------------------
We see that 'Unnamed: 0','cc_num','merchant','trans_num','unix_time','first','last','street','zip' are not Relevant
--------------------------------------------------------------------------------------------------------------------
We are only left with 14 Columns
--------------------------------------------------------------------------------------------------------------------
First we convert data and time column to date and time using pandas
--------------------------------------------------------------------------------------------------------------------
Then we Convert the date to -> Years , Months , Days
--------------------------------------------------------------------------------------------------------------------
Then we convert the upper converted Y-M-D and we convert it into paadas Dataframe
--------------------------------------------------------------------------------------------------------------------
Then we convert the Date of Birth to pandas dataframe
--------------------------------------------------------------------------------------------------------------------
Then we do the same with the testing dataset
--------------------------------------------------------------------------------------------------------------------
Calculate Age
--------------------------------------------------------------------------------------------------------------------
Train -> Now we are calculating the age of the person according to their date of birth and we save it in age column
--------------------------------------------------------------------------------------------------------------------
Get Transaction Month & Year
--------------------------------------------------------------------------------------------------------------------
Train -> Calculate distance between merchant and home location
--------------------------------------------------------------------------------------------------------------------
longitudnal distance = merch Longitude(Merch Location) - Longitue(Home Location)
--------------------------------------------------------------------------------------------------------------------
Still there are some columns that are now additional and we dont nedd them
--------------------------------------------------------------------------------------------------------------------
Dropping Columns that are not relevant to predicy fraud transaction
--------------------------------------------------------------------------------------------------------------------
Convert categorical column gender into numerical 
--------------------------------------------------------------------------------------------------------------------
For the Male it is 1 
--------------------------------------------------------------------------------------------------------------------
For Female it is 0
--------------------------------------------------------------------------------------------------------------------
One Hot Encoding of Category column
--------------------------------------------------------------------------------------------------------------------
Now we are again checking our file to find all the columns that we are working with and which we got 
--------------------------------------------------------------------------------------------------------------------
Such as Transaction Month , Age and Distance
--------------------------------------------------------------------------------------------------------------------
Now we have 23 Columns and 1296675
--------------------------------------------------------------------------------------------------------------------
Here now we are dropping is fraud from each row
--------------------------------------------------------------------------------------------------------------------
Fit the StandardScaler on the data
--------------------------------------------------------------------------------------------------------------------
Initialize and fit the Classifier on the training data
--------------------------------------------------------------------------------------------------------------------

2nd Project -> CUSTOMER CHURN using Classification Algorithms such as Gradient Boost 
--------------------------------------------------------------------------------------------------------------------
--------------------------------------------------------------------------------------------------------------------

We are first taking the Data for churn Modelling
--------------------------------------------------------------------------------------------------------------------
We are dropping the columns that are irrelevant such as 
Row Number , CustomerId , Surname
--------------------------------------------------------------------------------------------------------------------
Then we are going to encode the gender in our Dataset 
We took 0 for Male and 1 For the Female
Then we take the integer values
--------------------------------------------------------------------------------------------------------------------
As we can look from our data that the geography columns has different countries and we want to fit them
According to our model 
--------------------------------------------------------------------------------------------------------------------
By using Label Encoder we have encoded different Countries and assigned each one a number according to the label
--------------------------------------------------------------------------------------------------------------------
Then we are plotting a pie graph to see How much of our Customers have exited and how much are still there
--------------------------------------------------------------------------------------------------------------------
As we have calculated the Customers that have exited 
Now our goal is to drop them from our data as they will not be useful for our prediction
--------------------------------------------------------------------------------------------------------------------
Here we are counting the number of zeroes and ones and sampling the distribution class before oversampling
Then we used Random over sampler
Object to over-sample the minority class(es) by picking samples at random with replacement. The bootstrap can be generated in a smoothed manner.
--------------------------------------------------------------------------------------------------------------------
Standarizing the data by using (X= X - mean of X)/(standard Deivation of x)
--------------------------------------------------------------------------------------------------------------------
Now we are Splitting the training and testing data
Here we took the test size as 30%
--------------------------------------------------------------------------------------------------------------------
Our model is XGBoost (Gradient Boosting)
--------------------------------------------------------------------------------------------------------------------

