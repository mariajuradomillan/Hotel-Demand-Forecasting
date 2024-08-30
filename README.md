# Hotel Demand Forecasting

This repository contains the code and data for a project focused on forecasting hotel demand for a hotel located in the Algarve region of Portugal. The project uses various classification methods, including classical statistical models and advanced machine learning algorithms, implemented in R.

## Project Overview

Accurate demand forecasting is crucial in the hospitality industry to optimize resource management, enhance customer satisfaction, and improve operational efficiency. This project aims to predict hotel bookings using different models like Logistic Regression, Random Forest, and Gradient Boosting. After evaluating several models, Logistic Regression emerged as the top performer with a precision of 84.43% and a recall of 92.61%.

### Key Features:

-   Forecasting hotel demand using machine learning techniques.
-   Evaluating model performance with multiple metrics: Accuracy, Precision, Recall, and F1-Score.
-   Detailed descriptive analysis of the data to understand booking patterns and trends.

## Installation

To run this project, you need to have R and RStudio installed on your machine. You can download R from [CRAN](https://cran.r-project.org/) and RStudio from [here](https://rstudio.com/products/rstudio/download/).

Data can be downloaded from this [link](https://www.sciencedirect.com/science/article/pii/S2352340918315191?via%3Dihub).

### Required Packages

You can install the required R packages by running the following code:

---
packages <- c( "tidyverse", "dplyr", "readr", "plotly", "caret", "mice", "ggplot2", "gghighlight", "hrbrthemes", "patchwork", "leaflet", "MASS", "xgboost", "GGally", "factoextra", "rpart", "gt") 
# Install packages if they are not already installed
 install_if_missing <- function(package) { if (!require(package, character.only = TRUE)) { install.packages(package) library(package, character.only = TRUE) } } 
# Apply the function to all listed packages 
lapply(packages, install_if_missing)
---

## Usage

To run the analysis and train the models, follow these steps:

1.  Clone the repository:

    `git clone https://github.com/mariajuradomillan/Hotel-Demand-Forecasting.git`

2.  Navigate to the project directory:

    `cd Hotel-Demand-Forecasting`

3.  Open the R script in RStudio:

    `open Hotel-Demand-Forecasting.rmd`

4.  Load the data by modifying the `data <- read.csv("path/to/your/dataset.csv")` line in the script.

5.  Run the script to preprocess the data, train the models, and evaluate their performance.

## Results

The results of the analysis show that the Random Forest model achieved the highest accuracy (85.01%), while Logistic Regression had the highest recall (92.61%). Below is a summary of the best-performing models for each metric:

| Metric    | Model               | Value  |
|-----------|---------------------|--------|
| Accuracy  | Random Forest       | 85.01% |
| Recall    | Logistic Regression | 92.61% |
| Precision | Logistic Regression | 84.43% |
| F1-Score  | Logistic Regression | 88.34% |

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.
