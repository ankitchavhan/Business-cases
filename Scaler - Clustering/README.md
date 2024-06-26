# Scaler - Clustering

## Problem Statement

Scaler is an online tech-versity offering intensive computer science & Data Science courses through live classes delivered by tech leaders and subject matter experts. The meticulously structured program enhances the skills of software professionals by offering a modern curriculum with exposure to the latest technologies. It is a product by InterviewBit.

You are working as a data scientist with the analytics vertical of Scaler, focused on profiling the best companies and job positions to work for from the Scaler database. You are provided with the information for a segment of learners and tasked to cluster them on the basis of their job profile, company, and other features. Ideally, these clusters should have similar characteristics.

## Data Dictionary:

- ‘Unnamed 0’ - Index of the dataset
- Email_hash - Anonymised Personal Identifiable Information (PII)
- Company_hash - This represents an anonymized identifier for the company, which is the current employer of the learner.
- orgyear - Employment start date
- CTC - Current CTC
- Job_position - Job profile in the company
- CTC_updated_year - Year in which CTC got updated (Yearly increments, Promotions)

## Concept Used:
- Manual Clustering
- Unsupervised Clustering - K- means, Hierarchical Clustering

## What does “good” look like?
1. Import the dataset and do usual exploratory data analysis steps like checking the structure & characteristics of the dataset
2. Checking unique emails and frequency of occurrence of the same email hash in the data. Recording observation and inference, wherever necessary.
3. Checking for missing values and Prepare data for KNN/ Mean Imputation.
4. You may have to remove special characters from the dataset by using Regex
   - Don’t worry if you haven’t used that before. The syntax is quite simple and intuitive
   - Code:
     mystring='\tAirtel X Labs'
     re.sub('[^A-Za-z0-9 ]+', '', mystring)
5. Checking for duplicates in the dataset and drop them
6. Making some new features like adding ‘Years of Experience’ column by subtracting orgyear from current year
7. ***Manual Clustering*** on the basis of learner’s company, job position and years of experience
- Getting the 5 point summary of CTC (mean, median, max, min, count etc) on the basis of Company, Job Position, Years of Experience
- Merging the same with original dataset carefully and creating some flags showing learners with CTC greater than the Average of their Company’s department having same Years of Experience - Call that flag designation with values [1,2,3]
- Doing above analysis at Company & Job Position level. Name that flag Class with values [1,2,3]
- Repeating the same analysis at the Company level. Name that flag Tier with values [1,2,3]
8. Based on the manual clustering done so far, answering few questions like:
 - Top 10 employees (earning more than most of the employees in the company) - Tier 1
     - Top 10 employees of data science in each company earning more than their peers - Class 1
     - Bottom 10 employees of data science in each company earning less than their peers - Class 3
  - Bottom 10 employees (earning less than most of the employees in the company)- Tier 3
  - Top 10 employees in each company - X department - having 5/6/7 years of experience earning more than their peers - Tier X
  - Top 10 companies (based on their CTC)
  - Top 2 positions in every company (based on their CTC)
9. Data processing for Unsupervised clustering - Label encoding/ One- hot encoding, Standardization of data
10. Unsupervised Learning - Clustering
    - Checking clustering tendency
    - Elbow method
    - K-means clustering
    - Hierarchical clustering (you can do this on a sample of the dataset if your process is taking time)
11. Insights from Unsupervised Clustering
12. Provide actionable Insights & Recommendations for the Business.
