# Readme.md

## Objective

This project advances the work done in project [Prosper-Loan-Data-Exploration](https://github.com/udaygoel/Data-Analyst-Udacity/tree/master/Prosper-Loan-Data-Exploration) by illustrating the key drivers used by Prosper to determine the borrow rate for the loans and visualizing the change in relationship between these drivers over time. 

## Features Selection

For visualization, the features EstimatedLoss, Term (of loan) and the Loan Amount have been used as they represent, as a combination, both the borrower and loan dependent factors. It was found that these relationships have become much more strongly defined over the years, with a strong positive relationship between the borrow rate and EstimatedLoss. This also co-incides with a much higher new loan origination after initial couple of years. The relationship with Term has switched in 2013 with longer term loans being cheaper for the same EstimatedLoss. The biggest loan sizes are concentrated in the middle range of borrow rate.

## Design

The analysis in [Prosper-Loan-Data-Exploration](https://github.com/udaygoel/Data-Analyst-Udacity/tree/master/Prosper-Loan-Data-Exploration) showed that EstimatedLoss is the most important driver of the Borrow Rate, followed by the loan amount and finally the term. All the three set of value are continuous and since they exhibit correlation, a bubble chart has been used. These are visual encodings for the design:

1. EstimatedLoss on the x-axis
2. Borrow Rate on the y-axis 
3. Loan Original Amount as size of bubble
4. Term using sequential colours as the terms (12, 30, 60) are ordered
5. Year of Loan Origination, that is, Time, as animation

## Visualization

The visualization starts with an animation and shows how the relationship between the Borrow Rate and the 3 variables changes over each year. Special attention should be given to 2013 where the relationship between Borrow Rate and Term changes. At the start of 2013, 60 months loans have higher Borrow Rate than 36 months loans. This reverses by the end of 2013. This movement is shown by breaking 2013 into 4 quarters. 

The visualization switches to interactive mode at the end of animation. The user can select a particular year (or quarter for 2013) or change the x-axis scales.

The visualization is designed to show the bubbles in order of their size. The Loan Original Amount is split into 4 parts, in the order of value. The part with the smallest Loan Original Amount, that is, smallest bubbles, show first, followed by the next bigger bubble sizes. This has been done to ensure the user is able to see the placement of the small loan sizes in case they are overlapped by other bigger loans. Due to the number of loans, it is not possible to use only the transparency of the bubbles to show the placement of smaller bubbles.

The visualization can be seen here:

http://bl.ocks.org/udaygoel/raw/d3952e32da6cc30932a3c00b1e5f65bb/
Gist Location for the data and visualization: 

https://gist.github.com/udaygoel/d3952e32da6cc30932a3c00b1e5f65bb

#### Run Visualization Locally

To run the files from Gist on the local machine, these steps should be followed:

- Download the files in a destination folder. Unzip them if needed

- Open a command window (Terminal for Mac) and navigate to the destination folder

- We need to specify this folder as the localhost location. With Python 3.+, you this command:

  python -m http.server

  The default port should be 8000

- Launch web browser and type http://localhost:8000/

  The visualization should start in the browser

## Credit

Many thanks to Lavina Aggarwal, Rohit Goel and Paras Kothari for providing valuable feedback to improve the visualization.

## Resources

[1] [Prosper-Loan-Data-Exploration](https://github.com/udaygoel/Data-Analyst-Udacity/tree/master/Prosper-Loan-Data-Exploration)
[2] Prosper Loan Data - Variable Definitions: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0
[3] Colors for Term: 
http://colorbrewer2.org/#type=sequential&scheme=OrRd&n=3 
[4] Using Dictionary in JavaScript:
http://pietschsoft.com/post/2015/09/05/JavaScript-Basics-How-to-create-a-Dictionary-with-KeyValue-pairs
[5] Setting Axis Labels:
http://bl.ocks.org/phoebebright/3061203
[6] How to add legend to explain bubble size:
https://dojo.domo.com/t5/Card-Building/Displaying-what-controls-bubble-size-on-a-bubble-chart/td-p/28958
[7] Adding line with d3.js:
https://www.dashingd3js.com/svg-basic-shapes-and-d3js
