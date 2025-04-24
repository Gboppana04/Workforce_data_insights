<div align="center">
  <h1>📊 Data-Driven Insights into Employee Attrition, Salaries, and Performance Ratings</h1>
</div>

## 🔍 Overview
- Employee retention, fair compensation, and performance management are key to organizational success, but predicting which employees are at risk of leaving or understanding salary and performance trends can be challenging.

- This project tackles these issues head-on by analyzing 1,470 employee records. Using statistical techniques and data visualizations in R, we uncover insights into employee attrition, salary distribution, and performance ratings. These findings help HR professionals make data-driven decisions that reduce turnover, optimize compensation, and enhance performance.

## 📁 Dataset
- **Source**: [Kaggle - Employee Attrition Dataset](https://www.kaggle.com/datasets/patelprashant/employee-attrition)
- **Size**: 1,470 rows × 28 columns
- **Variables**: Includes demographic info, job role, satisfaction levels, performance ratings, salary details, and more.

# 🚀 Installation

To get started with this project, follow the steps below:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Gboppana04/Workforce_data_insights.git
    ```

2. **Install dependencies**:
    Open your R console or RStudio and run the following command to install the required packages:
    ```R
    install.packages(c("ggplot2", "dplyr", "car", "psych", "stats", "tidyverse"))
    ```

3. **Ensure R is installed**:
    Make sure that you have R installed on your system. You can download it from [CRAN](https://cran.r-project.org/).

4. **Set up a suitable IDE**:
    It's highly recommended to use RStudio for a smooth development experience. You can download it from [RStudio's website](https://posit.co/download/rstudio-desktop/).

Once the dependencies are installed and your environment is set up, you're ready to start using this repository.

# 💻 Usage

To run the analysis and reproduce the results, follow the steps below:

1. **Load the dataset and libraries**:
    Open an R console or RStudio, then load the necessary libraries and dataset:
    ```R
    library(ggplot2)
    library(dplyr)
    # Load other libraries as needed
    data <- read.csv("employee_attrition.csv")
    ```

2. **Run the analysis**:
    To analyze the data for all three research questions, run the single R Markdown script:
    - Open the [Attrition_code_book.Rmd](https://github.com/Gboppana04/Workforce_data_insights/blob/main/Attrition_code_book.Rmd) file in RStudio.
    - Click on the "Knit" button to generate the output. This will run all the necessary steps for data cleaning, analysis, and visualizations related to employee attrition, salaries, and performance ratings.

3. **View the output**:
    The results and visualizations will be generated in the output folder (or the default directory), where you can review the findings.

Follow these steps to run the analysis and explore the insights from the dataset.


## 🧪 Objectives
- 💰 What drives employee salaries?
- 🚪 What predicts employee attrition?
- 📈 What influences performance ratings?

## 🧼 Data Preparation
- Loaded and cleaned the dataset in R (`read.csv`)
- Checked for missing values, duplicates (none found)
- Addressed outliers using Winsorization and visualized via box plots
- Transformed non-normal variables (e.g., salary) using log transformation

## 📊 Exploratory Data Analysis
- Summarized key metrics (mean, median, std dev) across variables
- Normality tested using Shapiro-Wilk, Q-Q plots, and histograms
- Visualized distributions before and after transformation
- Performed correlation matrix and Fisher's Exact Test for categorical variable associations

## 📈 Statistical Modeling

We explored three core questions using statistical modeling in R:

## 🎯 Research Question 1: What drives employee salaries?
We applied **multiple linear regression** to assess how job role, job level, department, and performance ratings impact salaries. The final model explained **86% of salary variance (R² = 0.86)**, with job level and department emerging as strong predictors.

## 🎯 Research Question 2: What predicts employee attrition?
Using **logistic regression**, we found significant links between attrition and factors like job level, salary hikes, and job satisfaction. Oversampling improved class balance and model performance.

## 🎯 Research Question 3: What influences performance ratings?
We applied **OLS regression** to evaluate satisfaction and work-life factors. These showed limited impact, but **percentage salary hike** had a strong positive correlation (r = 0.77) with performance ratings. Alternative modeling may be more suitable for this outcome.

👉 [See full report here (Attrition_report.pdf)](https://github.com/Gboppana04/Workforce_data_insights/blob/main/Attrition_report.pdf) or explore the code in the [Attrition_code_book.Rmd](https://github.com/Gboppana04/Workforce_data_insights/blob/main/Attrition_code_book.Rmd).

These research questions guide the development of statistical models, ensuring we derive meaningful insights into employee salaries, attrition, and performance ratings. The iterative approach in refining these models ensures their robustness and applicability in HR decision-making.


## 📌 Key Takeaways
- Employees with higher job levels, better performance, and specific department roles tend to earn more.
- Work-life balance and job satisfaction show strong associations with attrition.
- Properly cleaning and transforming data significantly improved model performance.

## 🛠 Tools & Tech
- **Language**: R
- **Libraries**: ggplot2, dplyr, car, psych, stats, tidyverse
- **Techniques**: EDA, Regression Analysis, Data Transformation, Statistical Testing

## 🚀 Future Work
- Integrate machine learning models (e.g., decision trees, random forests) to improve prediction.
- Build interactive dashboards for HR analytics using Shiny or Power BI.
- Expand dataset with external economic or industry benchmarking data.


