
# Healthcare Expenditure Dynamics: An Exploratory Analysis

This project aims to conduct an exploratory data analysis on the "Medical Cost Personal Datasets" to understand the distribution and characteristics of the dataset, analyze relationships between various factors (such as age, BMI, smoker status, etc.) and medical costs, visualize the data, and create predictive models to estimate medical costs based on different attributes.

## Project Overview

- **Data**: The dataset used in this project was sourced from Kaggle and was originally published by the user 'mirichoi0218.' The dataset comprises 1338 records, each representing an individual's medical profile. It contains the following columns:
  - **Age**: The age of the individual.
  - **Sex**: The gender of the individual (male or female).
  - **BMI**: Body Mass Index, a measure of body fat based on height and weight.
  - **Children**: The number of children or dependents covered by the insurance.
  - **Smoker**: Whether the individual is a smoker (yes or no).
  - **Region**: The residential area of the individual in the US (northeast, northwest, southeast, southwest).
  - **Charges**: The medical costs billed by the health insurance.

## Project Structure

- `Healthcare Expenditure Dynamics.Rmd`: R Markdown file containing the project's code and analysis.
- `insurance.csv`: The dataset used for analysis.
- `Medical Cost Predictions.pptx`: Presentation summarizing the project findings.
- `project.R`: R script file with the project's analysis and modeling code.
- `.RData`: Workspace file with saved R environment.
- `.Rhistory`: File containing command history.
- `Healthcare Expenditure Dynamics.pdf`: PDF version of the analysis report.

## Objectives

The primary objectives of this project are as follows:
- Perform exploratory data analysis to understand the distribution and characteristics of the dataset.
- Analyze the relationships between various factors (age, BMI, smoker status, etc.) and medical costs.
- Visualize the data to gain insights into patterns and trends.
- Create predictive models to estimate medical costs based on different attributes.

## Tools and Libraries

The analysis and visualization were conducted using the R programming language with the following libraries:
- `tidyverse`: For data manipulation and visualization.
- `ggplot2`: For creating various types of data visualizations.
- `caret`: For building predictive models.

## How to Run

1. **Clone the repository**:
   git clone https://github.com/sandeeppandey1108/Healthcare-Expenditure-Dynamics.git
   

2. **Navigate to the project directory**:
   cd Healthcare-Expenditure-Dynamics
   

3. **Set up the virtual environment**:
   R -e "install.packages('renv'); renv::init()"

4. **Install the required dependencies**:
   R -e "renv::restore()"
   

5. **Run the R Markdown file**:
   
   R -e "rmarkdown::render('Healthcare Expenditure Dynamics.Rmd')"
   

## Analysis and Results

### Data Import and Preprocessing

- Imported the dataset and checked its structure and summary statistics.
- Converted categorical variables to factors.
- Checked for missing values and performed feature scaling.

### Exploratory Data Analysis

- **Histograms**: Created histograms for age and BMI to understand their distributions.
- **Box Plots**: Visualized medical charges by smoker status and region.
- **Bar Charts**: Analyzed the distribution of gender, smoker status, and region.
- **Scatter Plots**: Explored relationships between age, BMI, and medical charges, colored by smoker status.

### Statistical Analysis

- **T-tests**: Conducted t-tests to compare medical charges between smokers and non-smokers.
- **ANOVA**: Used ANOVA to compare medical charges across different regions.

### Predictive Modeling

- **Linear Regression**: Built a linear regression model to predict medical charges based on age.
- **Multiple Linear Regression**: Developed a multiple linear regression model using age, BMI, children, smoker status, sex, and region as predictors.
- **Logistic Regression**: Created a logistic regression model to predict smoker status based on age and charges.

### Model Evaluation

- Evaluated model performance using Mean Absolute Error (MAE) and Mean Squared Error (MSE).
- Visualized actual vs. predicted charges using scatter plots and box plots.

## Conclusions

The analysis provided valuable insights into the factors influencing medical costs. Significant relationships between medical charges and attributes like age, BMI, and smoker status were identified. Predictive models were developed to estimate medical costs based on these attributes. 

### Suggestions for the Project

- **Smoking Cessation Programs**: Considering the significant impact of smoking on medical charges, healthcare providers and policymakers should invest in smoking cessation programs and resources.
- **Regional Healthcare Policies**: Addressing regional variations in medical charges requires tailored healthcare policies and initiatives.

## Acknowledgments

- The dataset is provided by [Kaggle](https://www.kaggle.com/mirichoi0218/insurance).
- Special thanks to Professors Roberta Siciliano for their guidance.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
