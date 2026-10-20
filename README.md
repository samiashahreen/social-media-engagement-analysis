# social-media-engagement-analysis

1. Project Overview

This project investigates social media engagement patterns on Instagram and Facebook. It examines whether engagement differs by post type, posting time, and day of the week, and explores whether these factors can help predict engagement.

The purpose is to better understand patterns in social media engagement using exploratory data analysis and regression models.

2. Research Questions

This project addresses three research questions:

How does user engagement differ between different types of posts on Instagram and Facebook?

How does the time of day and day of the week a post is published impact user engagement on Instagram and Facebook?

To what extent can post type, time of day, day of the week, and social media platform be used to predict user engagement? 

3. Dataset Source

The data will be obtained from the University of Vienna Data Showcase, using the dataset by Lee et al. (2024).

Source: University of Vienna Data Showcase

Authors and year: Lee et al. (2024)

The dataset contains social media data from various social media platforms. Only data pertaining to Instagram and Facebook will be used. The data will be inspected to confirm the available variables, engagement measures, and suitability for answering the research questions.

See data/README.md for dataset access.

4. Planned Approach

Data Filtering and Preparation: Filter the full dataset to retain only Instagram and Facebook records. Inspect the relevant variables, check for duplicates, and prepare the data for analysis. Since the dataset contains no missing values, missing-value imputation will not be required.

Exploratory Data Analysis (EDA): Use descriptive statistics and visualizations to examine engagement patterns by platform, post type, posting time, and day of the week.

Comparative Analysis: Compare engagement across post types and investigate the relationship between posting time, day of the week, and engagement on Instagram and Facebook.

Predictive Modelling: Develop three regression models using platform, post type, posting time, and day of the week as predictors: Linear Regression as the baseline, Ridge Regression, and Random Forest Regression.

Model Evaluation: Compare the models using Mean Absolute Error (MAE) on the same held-out test set.

Reporting: Summarize the findings, answer the research questions, and discuss the limitations of the analysis.
