# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**:  https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/basic_pivot_charts.xlsx
- [x] **Solution**: https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/basic_pivot_charts_solution.xlsx

#### Learning Objective

Let's learn how to build basic pivot charts based on a disaggregated data.

#### Context

So far we have worked on summarized (aggregated) data but did you know that Excel is very efficient at visualizing disaggregated data? Pivot tables + pivot charts is a match made in heaven when it comes to visualizing lots of data points!

In this exercise, we learn how we can build insightful line and a bar charts using this technique!

##### STEP 1
- Load basic_pivot_charts.xlsx. 
- Create a pivot chart based on the data in sheet `Sample - Superstore` and place it in a new sheet called "Column and Line pivot charts".

##### STEP 2
- Visualize count of `Order ID` based per quarterly `Order Date` split by `Segment`.
- Present the result as a _line chart_.

##### STEP 3
Based on the same pivot table and in the same sheet, create another version of this chart, this time a _stacked column chart_.

##### STEP 4
Finally, beautify the pivot charts by adding a meaningful title and hiding all pivot buttons on the chart.

#### Exercise (open) question 1:
In which quarter we had the highest amount of Home Office orders? Provide an answer in format e.g. Q4-2010.

#### Exercise (open) question 2:
Which chart would you look at to check in which quarter we had overall the most orders? Type in either line or column.

#### Answer 1: 
Q1-2017

#### Answer 2: 
Column

#### End goal:
![image](https://github.com/AgataBG/sme-bi-course-application/assets/95186405/fe9cd61b-d159-4571-90fc-bd9543b7bb4b)


## 2nd VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**:  https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/slicer_and_timeline.xlsx
- [x] **Solution**: https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/slicer_and_timeline_solution.xlsx

#### Learning Objective

We will learn how to use visualizations actions and create an intuitive hover-over browser of titles per genre.

#### Context

Intuitive dashboard design is bringing us closer to better dashboard adoption among our end-users. 
Did you know that with Tableau you can make visualizations actions that will generate outputs in other visualizations based on selections or hovering over?
Let's get to it!

##### STEP 1
Load ex_2_2_2_hover_browser.twbx and create a new sheet called "Top Titles".

##### STEP 2
Filter on `Release Year` 2020 and build a table of `Title` with two measures: summed `IMDB Votes` and an average of `IMDB Score`.
Sort by highest `IMDB Votes` but also hide this column from the visualization.

##### STEP 3
Present the `IMDB Score` as a number with one decimal, apply color and "Square" `Marks Card` to change the visualization to resemble a heatmap. Adapt the solor scale to 10-step Red-Green diverging.
Change the title of the visualiztion to "Top Titles (by IMDB Votes) and their IMDB score".

##### STEP 4
Create a Dashboard called "Title browser" and place the `Word cloud` sheet on the left and our newly created `Top Titles` sheet on the right. 
Expand the `Word cloud` object visualization to "Entire View" and `Top Titles` to "Fit Width". 

##### STEP 5
Using the "Dashboard" and "Actions menu" create a new _Filter_ action which, by hovering over the genres in 'Word cloud' will present the top titles in 'Top Titles' visualization.

#### Exercise question:
What is the best romance Title of 2022, considering the IMDB score?

#### Answer:
The Baker and the Beauty

#### End goal:

<img width="1120" alt="2022-07-01 14_37_52-Tableau Public - DV - VM2 2 2 START" src="https://user-images.githubusercontent.com/95186405/176898089-e766e23d-ff45-4e35-b560-2453eec6c6fc.png">

