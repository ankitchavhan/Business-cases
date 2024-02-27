## OLA - Ensemble Learning Business Case
### The company’s perspective:
 - Ola is a leading ride-sharing platform, aiming to provide reliable, affordable, and convenient urban transportation for everyone.
 - The constant challenge Ola faces is the churn rate of its drivers. Ensuring driver loyalty and reducing attrition are crucial to thecompany's operation.
 - Analyzing driver data can reveal patterns in driver behavior, performance, and satisfaction. This would help in foreseeing potentialchurn, allowing proactive measures.
 - By leveraging data science and ensemble learning, Ola can predict driver churn, which would be pivotal in its driver retentionstrategy.
### Dataset Explanation: ola_driver.csv
1. MMMM-YY: Reporting month and year.
2. Driver_ID: A unique identifier for every driver.
3. Age: Age of the driver.
4. Gender: Driver's gender. Male: 0, Female: 1.
5. City: City code representing the city the driver operates in.
6. Education_Level: Education level of the driver, categorized into 0 for 10+, 1 for 12+, and 2 for graduate.
7. Income: Average monthly income of the driver.
8. Date Of Joining: The date when the driver joined Ola.
9. LastWorkingDate: The most recent or final day the driver worked with Ola.
10. Joining Designation: Designation of the driver at the onset of their journey with Ola.
11. Grade: A grade assigned to the driver at the reporting time, likely denoting performance or other metrics.
12. Total Business Value: The total monetary value (business) a driver brings in a month. Negative values might indicate cancellations,refunds, or other financial adjustments.
13. Quarterly Rating: Rating assigned to drivers on a quarterly basis. Ratings range from 1 to 5, with 5 being the best.

### Problem Statement
Assuming you are a data scientist at Ola, you are entrusted with the responsibility of analyzing the
dataset to predict driver attrition (reduction). Our primary goal is to utilize ensemble learning
techniques, evaluate the performance of your models, and provide actionable insights to reduce driver
churn
