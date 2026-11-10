# Social Media Engagement Analysis

## 1. Project Overview

This project investigates social media engagement patterns on Instagram and Facebook. It examines whether engagement differs by post type, posting time, and day of the week, and explores whether these factors can help predict engagement.

The purpose is to better understand patterns in social media engagement using exploratory data analysis and regression models.

## 2. Research Questions

This project addresses three research questions:

1. How does user engagement differ between different types of posts on Instagram and Facebook?
2. How does the time of day and day of the week a post is published impact user engagement on Instagram and Facebook?
3. To what extent can post type, time of day, day of the week, and social media platform be used to predict user engagement?

## 3. Dataset Source

The data is obtained from the University of Vienna Data Showcase, using the dataset by Lee et al. (2024).

- **Source:** University of Vienna Data Showcase
- **Authors and year:** Lee et al. (2024)

The dataset contains social media data from various social media platforms. Only data pertaining to Instagram and Facebook will be used. The data is inspected to confirm the available variables, engagement measures, and suitability for answering the research questions.

See `data/README.md` for dataset access information.

## 4. Project Methodology and Stages

### Stage 1: Data Filtering and Preparation

Filter the full dataset to retain only Instagram and Facebook records. Inspect the relevant variables, check for duplicates, and prepare the data for analysis. Since the dataset contains no missing values, missing-value imputation is not required.

### Stage 2: Exploratory Data Analysis (EDA)

Use descriptive statistics and visualizations to examine engagement patterns by platform, post type, posting time, and day of the week.

### Stage 3: Comparative Analysis

Compare engagement across post types and investigate the relationship between posting time, day of the week, and engagement on Instagram and Facebook.

### Stage 4: Predictive Modelling

Develop three regression models using platform, post type, posting time, and day of the week as predictors:

- **Linear Regression:** Baseline model.
- **Ridge Regression:** Regularized linear regression model.
- **Random Forest Regression:** Tree-based ensemble model.

### Stage 5: Model Evaluation

Evaluate and compare model performance using Mean Absolute Error (MAE) on the same held-out test set. Interpret the results and identify the strengths and limitations of each model.

### Stage 6: Reporting and Interpretation

Summarize the findings, answer the research questions, and discuss the limitations of the analysis.

## 5. Repository Structure

The repository is organized into the following folders and files:

```text
social-media-engagement-analysis/
│
├── data/
│   └── README.md
│
├── notebooks/
│   └── WIP_Social_Media_Engagement_Analysis.ipynb
│
├── reports/
│   └── Social_Media_Engagement_Analysis.pdf
│
├── .gitignore
└── README.md
```

- **data/**: Contains dataset access information and instructions.
- **notebooks/**: Contains the Jupyter Notebook with the technical analysis, code, visualizations, and model development.
- **reports/**: Contains the compiled PDF version of the technical analysis.
- **.gitignore**: Specifies files and folders excluded from version control.
- **README.md**: Provides an overview of the project, methodology, repository structure, and execution instructions.

## 6. Technologies and Libraries

The project uses Python and the following libraries:

- **Pandas:** Data manipulation and analysis.
- **NumPy:** Numerical operations.
- **Matplotlib:** Data visualization.
- **Seaborn:** Statistical data visualization.
- **Scikit-learn:** Data preprocessing, regression modelling, and model evaluation.

## 7. How to Run the Project

The analysis is conducted using Python in Google Colab.

To reproduce the analysis:

1. Clone or download this GitHub repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload or open the Jupyter Notebook from the `notebooks/` folder.
4. Obtain the dataset using the instructions in `data/README.md`.
5. Upload the dataset when prompted by the notebook.
6. Run the notebook cells sequentially from beginning to end.

Ensure that the required Python libraries are available in the execution environment before running the notebook.

## 8. Reproducibility and Code Quality

The project uses a structured analytical workflow to support reproducibility and maintainability.

- A fixed random state of 42 is used for the train-test split to support reproducible results.
- Data preprocessing and categorical encoding are implemented using Scikit-learn.
- A preprocessing pipeline is used to maintain consistent transformations between training and testing data.
- Code comments and Markdown explanations document the analytical steps and modelling decisions.

## 9. Project Status

The project is being developed in stages. The current submission focuses on data exploration, preprocessing, and baseline Linear Regression development and evaluation. Additional regression models and comparative evaluation will follow in subsequent project stages.
Reporting: Summarize the findings, answer the research questions, and discuss the limitations of the analysis.
