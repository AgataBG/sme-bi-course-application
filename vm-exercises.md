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

So far we have worked on a summarized (aggregated) data but did you know that Excel is very efficient at visualizing disaggegated data? Summarizing the data with pivot tables and visualizing then with pivot charts, we can bring insightful graphs and adapt them in no time!
In this exercise we will build a line and a bar chart using this technique!

##### STEP 1
- Load basic_pivot_charts.xlsx. 
- Create a pivot chart based on the data in sheet `Sample - Superstore` and place it in a new sheet called "Column and Line pivot charts".

##### STEP 2
- Visualize count of `Order ID` based per quarterly `Order Date`.
- Present the result as a _line chart_.

##### STEP 3
- Create a separate sheet called `Actors` and construct a table of `Name` and the count of `Title ID`.
- Filtering `Role` on "ACTOR" and `Name` on Top 1 Actor based on the measure.
- Simplify the visualization of the table by removing borders and suffixing the count with " films".

##### STEP 4
- In `Word Cloud` sheet, adapt the `Tooltip` to display "Top actor" and the name of the actor. 
- You will need to add some of the filters to the context in the `Actors` sheet.

##### STEP 5
- Add the title to your visualization and a subtitle informing the user that he can check-out the name of the most popular actor by hovering over the genre.
- Style your output (color, size, font) according to your esthetics.

#### Exercise question:
What is the first name of the actor who starred in most Comedy titles of all times? 

#### Answer:
Eric

#### End goal:
<img width="962" alt="2022-07-01 13_56_03-Tableau Public - DV - VM2 2 1 END" src="https://user-images.githubusercontent.com/95186405/176889888-4164b0a5-45c2-488b-9fe5-47d7fe19c251.png">


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

