
# Analyze A/B Test Results E-commerce Website

## Packages Required
* Pandas
* Numpy
* random
* matplotlib
* seaborn
* statsmodesls.api 

## System and Software Requirement
* Python 3
* Ram - 2GB minimum
* Notebook - Jupyter 
* Anaconda

## Intrdouction
In this project I used the following statistical methods to give suggestions for the ecommerce website
* Probability
* A/B Test Results 
* Regression

### About the Data
* Number of rows and columns (294478,5)
* Variables --> user_id,timestamp, group, landing_page, converted
* user_id is the ID's for the Users
* timestamp--> The time they are using the page 
* group--> control or treatment group (control means for old_page , treatment means for new_page)
* landing_page --> What type of page (old_page or new_page)
* converted --> 0 means not converted , 1 means converted 

### Results
* Probability --> As we cleaned the data (the treatment group --> new_page & the contol group --> old_page) this means the result will be accurate. We can see that 50% of users are recieveing new_page and the conversion rate is 11.8%
  As the data is approximately 50-50 divided we can also say that control group users will see the old_page and their conversion rate is 12.03%
  From this we can see that old_page is having better slightly new_page as the difference is small we cannot say that the new_page will not beneficial(practical significance)
  This analysis gives us an idea but it is not suufficient to decide whether the new_page will be better than old_page
* A/B Test--> Since the p_val(ie prop_diff_more) is equal to 0.90 and the alpha value is 0.05 as we took 5% Type 1 error. This means the p-value is greater than 0.05, hence we fail to reject Null Hypothesis. This means that there is no statistical difference between the users getting converted using the new page and the old page. As we use the built in function in the stats model we are getting the p-value is 0.905 and z-stat (zscore) to be 1.3109. If we compare the p-value in j it was 0.9035 and we were fail to reject null hypotheis as the p-value > apha value. Similar for the the rest of results by the above built in function the p-value > alpha (0.05) hence we fail to reject Null Hypothesis
* Regression --> The regression model above was based upon if a person falls in the traeatment group or control group and gets converted. It means the prediction will be dependent upon which group the person is assigned. This makes the model not accurate and we see that from the p-value of ab_page making it not statistical significant. We could have added a duration column helping us to know how much time a users spends on the page before taking the decicsions. This will help us in making better decicion or deciding a better model. But adding more variables could increase the complexity like the duration can be related to group because if the page has some changes that reduces time then users with new group (treatment group) will be related. For eg: If you fall under treatment you will get converted. Yeah so for the correct model we need to see whats the accuracy,precicion of the model


```python

```
