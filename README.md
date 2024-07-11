# Vanguard A/B Test Experiment

## Overview
This project evaluates the impact of a new website layout on user experience and process completion rates at Vanguard. The dataset includes various user interaction details such as Client ID, Gender, Age, Number of Accounts per Client, Date and Time of Interaction, Visit ID, Balance, Client Tenure, Process Steps, and more.

## Goals
### The main objectives of this project are:

Assess if the new design improves user experience.
Determine if the new design increases process completion rates.

### Experiment Design
Period: March 15, 2017, to June 20, 2017.
Control Group: Clients interacted with Vanguard’s traditional online process.
Test Group: Clients experienced the new, enhanced digital interface.
Both groups followed the same sequence: an initial page, three steps, and a final confirmation page.

### Key Performance Indicators (KPIs)
Time Spent on Each Step: The average duration users spend on each step.
Completion Rate: The proportion of users who reach the final ‘confirm’ step.
Error Rates: Instances where users go back to a previous step, indicating confusion or an error. Transitioning from a later step to an earlier one is considered an error.

## Data Source
The dataset was collected from Vanguard's website interactions during the experiment period, providing comprehensive user interaction data to analyze the impact of the new website layout on user behavior.

## File Structure
notebooks/vanguard_experiment.ipynb: Jupyter notebook containing the main script for analyzing the A/B test results. \n
data/: Directory containing the dataset. \n
images/: Directory containing charts in .png format. \n
slides/: Directory containing information about the presentation. \n
README.md: This file providing an overview of the project. \n 

## Methodology
The dataset was cleaned to ensure accuracy and completeness, handling missing values and duplicates. Users who spent more than 30 minutes on any step in either group were excluded. The analysis primarily involved calculating averages and percentages for exploratory data analysis (EDA). Python and various libraries were utilized for data manipulation, visualization, and statistical analysis.

### Statistical Analysis
To validate the results, the following statistical tests were conducted:

Time Spent on Each Step: T-tests to determine if there is a significant difference in the average time spent on each step between the control and test groups.
Completion Rate: Z-tests to compare the completion rates between the control and test groups.
Error Rates: Z-tests to assess differences in error rates between the control and test groups.

## Results
### Time Spent on Each Step
Observed improvements include reduced time spent on each step in the test group.
### Completion Rate
The new design does not meet the company's threshold, as they expected a minimum 5% increase to justify the investment.
### Error Rates
Overall, errors decrease throughout the process, but the first step has a higher error rate than the control, potentially causing users to abandon the session early.
Despite some progress, the outcomes don't meet company standards, and the investment isn't justified.


## File Structure
- notebooks/vanguard_experiment.ipynb: Jupyter notebook containing the main script for analyzing the A/B test results. 
- data/: Directory containing the dataset. 
- images/: Directory containing charts in .png format. 
- slides/: Directory containing information about the presentation. 
- README.md: This file providing an overview of the project. 

## Technologies Used
This project is implemented in Python and utilizes various libraries for data analysis and visualization. Refer to the requirements-dev.txt file for the required libraries.

## Installation
To set up the project environment, install the required dependencies listed in the requirements.txt file.

pip install -r requirements.txt

## Contact Information
If you have any questions or issues, please contact me at joaosousa.sk8@gmail.com