# ITSM Incident Management
## ABC Tech

# Project Summary

### Requirement
ABC Tech is an organisation operating in IT-enabled business segment over a decade. On an average ABC Tech receives 22-25k IT incidents/tickets, which are handled to best practice by ITIL framework with incident management, problem management, change management and configuration management processes. ABC Tech management is looking for ways to improve the incident management process as recent customer survey results shows that incident management is rated as poor. Machine learning looks prospective to improve ITSM processes through prediction and automation.

They came up with 4 key areas, where Machine Learning can help ITSM processes in ABC Tech:
1. Predicting High Priority Tickets: To predict priority 1 & 2 tickets, so that they can take preventive measures or fix the problem before it surfaces.
2. Forecast the incident volume in different fields, quarterly and annual. So that they can be better prepared with resources and technology planning.
3. Auto tag the tickets with right priorities and right departments so that reassigning and related delay can be reduced.
4. Predict RFC (Request for change) and possible failure/misconfiguration of ITSM assets.

### Analysis
The data is ordinal, nominal as well as categorical. To analyze the data, various data processing techniques like Label Encoding and Standardization is used.For training the data and predicting the target, algorithms used are Support Vector Machine, Decision Tree, Random Forest, K-Nearest Neighbor, XGBoost Classifier and Artificial Neural Network. Volume Forecasting is done with the help of Statsmodels & Matplotlib.

The analysis is done in three parts:
1. Predicting Priorities: The predictor variables are Category, CI Category, CI Subcategory & WBS
2. Predicting Request for Change (RFC): The predictor variables are Category, CI Subcategory, WBS, Priority, Number of Related Interaction, Number of Related Incidents
3. Forecasting the Incident Volume: The predictor variable is opening time.

### Summary
   The project is done with the purpose of:
1. Finding out factors which affects priority and training a model which accurately predicts it so that preventive measures can be taken for High Priority Tickets and reassigning can be reduced.
2. Finding out factors which affect RFC and predicting it.
3. Forecasting Incident Volume in the future so that they can be better prepared with resources and technology planning.

The following steps are carried out:
1. Importing the data, necessary libraries, & exploring the data to look for missing values.
2. Selecting the features for analysis, label encoding the ordinal column and splitting the data into test & train.
3. Training the data using algorithms like Support Vector Machine, Decision Tree, Random Forest, K-Nearest Neighbor, XGBoost Classifier and Artificial Neural Network and checking the accuracy to find out which algorithm is the best.
4. Exporting the model with highest accuracy.
5. For Incident Volume Forecasting, Ticket Opening Time is taken and Time Series Forecasting is used.

### Results
For predicting Ticket Priority, Random Forest gives almost 98.5% accuracy. Predicting RFC accurately is not possible with this data. And Volume Forecasting is visualized with the help of Matplotlib throughout the year.
