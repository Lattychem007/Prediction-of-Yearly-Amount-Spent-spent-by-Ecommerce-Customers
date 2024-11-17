## Prediction-of-Yearly-Amount-Spent-spent-by-Ecommerce-Customers
![image](https://github.com/user-attachments/assets/d2ca1018-f098-40b3-af3f-593134048d6e)

# Problem Statement
Congratulations! You just got some contract work with an Ecommerce company based in New York City that sells clothing online but they also have in-store style and clothing advice sessions. Customers come in to the store, have sessions/meetings with a personal stylist, then they can go home and order either on a mobile app or website for the clothes they want.
The company is trying to decide whether to focus their efforts on their mobile app experience or their website. They've hired you on contract to help them figure it out! Let's get started!

# Processing Data
We'll work with the Ecommerce Customers csv file from the company. It has Customer info, suchas Email, Address, and their color Avatar. Then it also has numerical value columns:
-Avg. Session Length: Average session of in-store style advice sessions.
-Time on App: Average time spent on App in minutes
-Time on Website: Average time spent on Website in minutes
-Length of Membership: How many years the customer has been a member.
** Read in the Ecommerce Customers csv file as a DataFrame called customers.**

# Exploratory Data Analysis

**Using seaborn to create a jointplot to compare the Time on Website and Yearly Amount Spent columns to validate the correlation between each variables with our target

# Training and Testing Data
The data  split the data into training and testing sets. 
** Setting a variable X equal to the numerical features of the customers and a variable y equal to the "Yearly Amount Spent" column. **

# Predicting Test Data
Fitting  our model to evaluate its performance by predicting off the test values!

# Evaluating the Model
 Evaluation of   model performance by calculating the residual sum of squares and the explained variance score (R^2).

** Calculate the Mean Absolute Error, Mean Squared Error, and the Root Mean Squared Error. Refer to the lecture or to Wikipedia for the formulas**

# Conclusion
We still want to figure out the answer to the original question, do we focus our efforst on mobile app or website development? Or maybe that doesn't even really matter, and Membership Time is what is really important. Let's see if we can interpret the coefficients at all to get an idea.

 # Coeffecient
   - Avg. Session Length	25.981550
   
  - Time on App	38.590159
  
 -  Time on Website	0.190405
  
 -  Length of Membership	61.279097

# Interpreting the coefficients:

***Holding all other features fixed, a 1 unit increase in Avg. Session Length is associated with an increase of 25.98 total dollars spent.***
***Holding all other features fixed, a 1 unit increase in Time on App is associated with an increase of 38.59 total dollars spent.***
***Holding all other features fixed, a 1 unit increase in Time on Website is associated with an increase of 0.19 total dollars spent.***
***Holding all other features fixed, a 1 unit increase in Length of Membership is associated with an increase of 61.27 total dollars spent.***
**Do you think the company should focus more on their mobile app or on their website?**
***This is tricky, there are two ways to think about this: Develop the Website to catch up to the performance of the mobile app, or develop the app more since that is what is working better. This sort of answer really depends on the other factors going on at the company, you would probably want to explore the relationship between Length of Membership and the App or the Website before coming to a conclusion!**

