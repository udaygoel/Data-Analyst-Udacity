# Prosper-Loan-Data-Exploration
The objective of this project is to explore the data set of almost 114,000 loans with 81 variables from peer-to-peer lending firm [Prosper](https://www.prosper.com/). 

### Project Files

The project uses these files:

- prosperLoanData.csv: This csv has the data in a tabular form and forms the full dataset available for this project
- prosper_loan_exploration_by_udaygoel.Rmd: This R-Studio file contains the whole exploratory analysis of the data in R. The analysis includes the charts, observations and final conclusions.
- prosper_loan_exploration_by_udaygoel.html: This is the html output of the Rmd file.
- ScatterPlotMatrix.png: This is the scatterplot matrix used in Bivariate Analysis. It has been provided to allow a bigger view of the matrix. 

### Objective

The project conducts univariate, bivariate and multivariate analysis using several features to identify their relationship to the pricing of loans. The features can be taken directly from the dataset or engineered by running mathematical operations on a single or multiple features provided.

### Contents

There are 3 main sections of the Project.

1. Univariate Analysis

   This section analyses the structure of the dataset, creates new variables and identifies the relationships we wish to study.

2. Bivariate Plots Section

   Based on the Univariate Analysis, a subset of the dataset has been created with a reduced number of variables and a scatterplot matrix is produced. Multiple plots of different types are created to understand the relationships of interest. 

3. Multivariate Plots Section

   Learning from the analysis in the previous 2 sections, this section creates several multivariate plots to further understand the relationships. It then proceeds to develop a linear model that can explain 96.6% of the variation in the loan pricing. It also identifies the limitations of the approach.

4. Final Plots and Summary

   This section covers one plot and its description from each of the above section that provides the most interesting information in understanding the final result.

5. Reflection

   This section summaries the results and limitations of the analysis

### Citations

List of websites, books or other forums used:.

1. Use of mtable()

https://www.rdocumentation.org/packages/memisc/versions/0.99.14.9/topics/mtable

2. RColorBrewer, palette and use of colours with ggplot2

http://colorbrewer2.org/#

https://data.library.virginia.edu/setting-up-color-palettes-in-r/

http://www.sthda.com/english/wiki/ggplot2-themes-and-background-colors-the-3-elements#change-the-colors-of-the-plot-panel-background-and-the-grid-lines

 