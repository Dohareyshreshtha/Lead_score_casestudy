# Lead Score Case Study - X Education

## Problem Statement
X Education, an online course provider for industry professionals, aims to improve its lead conversion rate. Despite generating a significant number of leads, their conversion rate is low, at around 30%. To enhance the efficiency of their sales team, X Education seeks to identify high-potential leads, or "Hot Leads," so that the team can focus on the leads most likely to convert.

The goal is to build a logistic regression model to assign a lead score between 0 and 100 to each lead, where a higher score indicates a higher likelihood of conversion. The company has set a target conversion rate of approximately 80%.

## Objective
1. **Develop a Predictive Model**: Use logistic regression to predict the likelihood of lead conversion.
2. **Assign Lead Scores**: Create a lead scoring system where higher scores represent a higher probability of conversion.
3. **Handle Data Challenges**: Address issues such as categorical variables with the 'Select' level, which is akin to missing data.
4. **Enable Future Flexibility**: Ensure the model can adapt to potential changes in business requirements.

## Dataset
The dataset contains 9000 rows and multiple features, including:
- **Lead Source**: Origin of the lead (e.g., Google, direct traffic, referrals).
- **Total Time Spent on Website**: Duration a lead spends on the website.
- **Total Visits**: Number of times a lead visited the website.
- **Last Activity**: The last action performed by the lead.
- **Target Variable (Converted)**: 1 if the lead was converted into a paying customer, 0 otherwise.

### Data Issues
- Many categorical variables contain a 'Select' level, which represents missing information and needs to be treated accordingly.

## Process of Solving
1. **Data Cleaning and Preprocessing**:
   - Remove or treat the 'Select' level in categorical variables as missing values.
   - Handle null values and outliers.
   - Convert categorical variables into dummy variables for modeling.

2. **Exploratory Data Analysis**:
   - Univariate, bivariate, and multivariate analysis to identify patterns and relationships between features and the target variable (Converted).
   - Identify the most significant variables for lead conversion.

3. **Model Development**:
   - Split the data into training and test sets (e.g., 70:30).
   - Build a logistic regression model using the preprocessed data.
   - Evaluate the model using accuracy, precision, recall, F1-score, and ROC-AUC score.

4. **Assigning Lead Scores**:
   - Use the logistic regression model to assign a lead score between 0 and 100.
   - Sort leads by score, with the highest scores indicating "Hot Leads."

5. **Recommendation & Insights**:
   - Provide actionable insights to improve lead conversion rates.
   - Ensure the model is flexible enough to accommodate future business needs.

## Expected Results
- A logistic regression model capable of predicting lead conversion with high accuracy.
- A lead scoring system where leads with scores closer to 100 are the most likely to convert.
- Clear business recommendations based on model insights, helping the sales team focus on high-potential leads.
- Improved lead conversion rate towards the target of 80%.

## Recommendations
1. **Increase Focus on High-Potential Leads**: Prioritize leads with high lead scores for sales team outreach.
2. **Optimize Marketing Strategies**: Analyze lead sources and last activities to fine-tune marketing efforts.
3. **Enhance Lead Nurturing**: Improve communication and follow-up strategies for leads with mid-level scores to increase their conversion probability.

## Future Scope
- Fine-tuning the model with additional features or advanced techniques if business requirements change.
- Explore additional models (e.g., decision trees, random forests) to compare performance with logistic regression.
