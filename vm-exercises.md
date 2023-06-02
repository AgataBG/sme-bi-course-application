# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**:  https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/basic_pivot_charts.xlsx
- [x] **Solution**: https://github.com/AgataBG/sme-bi-course-application/blob/db3e386c7d4edcb4fb728933e40f5bad4dfa3ab2/exercises/basic_pivot_charts_solution.xlsx

#### Learning Objective

Let's learn how to build basic pivot charts based on disaggregated data.

#### Context

So far we have worked on summarized (aggregated) data but did you know that Excel is very efficient at visualizing disaggregated data? Pivot tables and pivot charts are a match made in heaven when it comes to visualizing lots of data points!

In this exercise, we learn how to build insightful line and column charts using this technique!

##### STEP 1
- Load basic_pivot_charts.xlsx. 
- Create a pivot chart based on the data in sheet `Sample - Superstore` and place it in a new sheet called "Column and Line pivot charts".

##### STEP 2
- Visualize the count of `Order ID` based on quarterly `Order Date`, split by `Segment`.
- Present the result as a _line chart_.

##### STEP 3
Based on the same pivot table and in the same sheet, create another version of this chart, this time a _stacked column chart_.

##### STEP 4
Finally, beautify the pivot charts by adding meaningful titles and hiding all pivot buttons on the chart.

#### Exercise (open) question 1:
In which quarter we had the highest amount of Home Office orders? Provide an answer in format e.g. Q4-2010.

#### Exercise (open) question 2:
Which chart provides a better answer to the question "In which quarter did we have the most orders overall"? Type in either line or column.

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

We will learn how to add interactivity to our pivot charts by using slicers and timelines.

#### Context

Pivot charts are so versatile, but they really come to life when connected with one another! We can add interactivity to our pivot tables and charts by adding _slicers_ (which you have already seen in action in the demo) as well as _timelines_, which can be used with any date fields. They both act as interactive filters and bring us one step closer to building mini Excel dashboards. 

Let's see it all in action!

##### STEP 1
Load slicer_and_timeline.xlsx, duplicate the sheet `Column and Line pivot charts` and call it "Slicer and Timeline".

##### STEP 2
Did you know that we can add any data column a _Slicer_, even if it's not present in our pivot table and chart?
- Add a _Slicer_ based on `State` field and test it out.
- Investigate various slicer options in _Slicer_ menu and make sure that the states are appearing in two columns.

##### STEP 3
Next, we will add a _timeline_, the same way as you would add a _slicer_. Since it is a date-based filter, make sure to select a relevant `Order...` field as the basis for it.

##### STEP 4
Adapt the _timeline_ to the same date dimension (year/quarter/month etc.) as currently is present in the pivot table and test it out.

#### Exercise question:
Using your interactive filters, zoom in on the period of Q1-2018 till Q4-2019 and find out for (jointly) California, New York and Pennsylvania states which quarter delivered the least orders. Provide an answer in format e.g. Q4-2010.

#### Answer:
Q3-2019

#### End goal:

![image](https://github.com/AgataBG/sme-bi-course-application/assets/95186405/20d7759a-f1a3-4f10-8908-adae04c65a88)

