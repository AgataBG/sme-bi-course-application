# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**:  https://github.com/AgataBG/sme-bi-course-application/blob/master/exercises/ex_2_2_1_word_cloud.twbx 
- [x] **Solution**: https://github.com/AgataBG/sme-bi-course-application/blob/master/exercises/ex_2_2_1_word_cloud-sol.twbx

#### Learning Objective

Let's learn how to build a word cloud chart and use the tooltip to provide extra information!

#### Context

A word cloud chart, also known as tag cloud, is a vusualization consisting of (key) words relevant to the dataset and enriched with measures (e.g. based on importance) by means of size or color of the individual words.
In this exercise we will build a word cloud to understand the importance of various genres in Netflix Movies and Series dataset and we will build in a tooltip providing the name of the most popular actor of the genre.

##### STEP 1
Load ex_2_2_1_word_cloud.twbx. The sheet `Word Cloud` already contains the `Genre (main)` dimension in `Rows`.

##### STEP 2
- Move the `Genre (main)` dimension from `Rows` onto `Text Marks Card` and apply a distinct count of `Title ID` onto size.
- Notice that the chart will automatically change to `Treemaps`. Adapt the `Marks` to switch it back to `Text`.

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
