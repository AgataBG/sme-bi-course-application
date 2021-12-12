# Virtual Machine (VM) Exercises

## :information_source: Read this before getting started
- The two exercises should not replicate the exact actions shown in your screencast. The goal of exercises is for learners to apply what was learned in the screencasts to new problems or situations. This is best pedagogical practice for retaining and building skills. For example, this can be done by using another dataset between screencasts and exercises or focusing on a different portion of the dataset.
- We can only run free versions of BI software in our virtual machine exercises. In the case of Power BI, make sure the exercises can run on [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) without any additional paid products. 
- Unsure what the scope of an exercise should be? Here's an [example](https://campus.datacamp.com/courses/introduction-to-power-bi/getting-started-with-power-bi?ex=14) from Introduction to Power BI. The first chapter of most DataCamp courses are free, so take a look at our [BI courses](https://learn.datacamp.com/courses?technologies=Tableau&technologies=Power%20BI) to get a feel for how we assess and guide learners.

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
- [x] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix`

#### Learning Objective

Let’s test your understanding of INCLUDE Level of Expression function in practice!

#### Context

INCLUDE Level of Detail (LOD) Expression is very useful when we need to navigate between various levels of granularity in our data, for example, having data on daily, hourly and per minute basis and perform calculations between these levels. It allows us to tap into various dimensions without explicitly dropping them into the visualization. Let's explore FitBit Heart Rate data to analyse differences between users’ average per minute and maximum per day Heart Rates.

#### Steps to be executed by the student (max 6)

##### STEP 1
- Load 2_1_HR.twbx [ex_1_initial.twbx] workbook. FitBit UserIDs and their categories are already placed on Rows.
- Add Heart Rate per Minute to Columns and apply Average aggregation to it.
- Filter out usage with no data by right-clicking on this measure in Columns, selecting Filter, last option Special and selecting only non-null values and Apply.

##### STEP 2
- Create a new calculated field (Level of Detail expression), called Heart Rate per Day, based on average Heart rate per Minute including Heart Rate Day Date dimension in the calculation.
- Drop your new measure Heart Rate per Day to Columns and change the aggregation to Average.
- Grab Heart Rate per Day one more time from the field list and drop it again to Columns, next to your Average Heart Rate per Day, but change the aggregation to Maximum on this second one. 

##### STEP 3
- Convert your visualization to side-by-side chart using Show Me.
- Rotate your chart by clicking on Swap Rows and Columns button.
- Let’s focus on Casual Exercisers: filter out all other User Categories.
- Expand your canvas to Entire view.


#### Exercise question:
Which Casual Exerciser has the largest difference between Maximum and Average Daily Heart Rates?
Give his/hers FitBit User ID (10 digit number).

#### End goal:

<img width="281" alt="image" src="https://user-images.githubusercontent.com/95186405/145714216-d56c1672-8e3a-469c-9a10-a34025bd9c32.png">

## 2nd VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

#### Files

- [x] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-2-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
- [x] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix`

#### Learning Objective

Expand the knowledge of INCLUDE LOD expression in practice and use it with multiple dimensions!

#### Context

Did you know that you can use more than one dimension in INCLUDE clause? Being able to calculate freely across dimensions without placing them in the canvas opens new horizons for our visualizations. Let’s see how it works, based on your knowledge so far, it should be a piece of cake! We will build further on our previous exercise from this lesson.

#### Steps to be executed by the student (max 6)

##### STEP 1
- Load 2_1_HR_And_Sleep.twbx [ex_2_initial.twbx] workbook. Our previously calculated average Heart Rate per Day (LOD) per user is placed on the Columns.
- Let’s change this LOD calculation to Heart Rate per Hour.
- To do so, edit it in the Field list, and change the dimension argument from Heart Rate per Day Date to Heart Rate Hour and rename your adapted field.
##### STEP 2
- Create a new calculated field called Steps per Day (LOD), based on Sum of No of Steps per Hour including Steps Day Date dimension in the calculation.
- Place it on Columns and aggregate by Average. Add mark labels on both graphs.
##### STEP 3
- Let’s go ahead and color both graphs by User Category  - go to Marks All and drag User Category from the field list onto color.
- Now, let’s try to remove FitBit User IDs from the Rows, to obtain averages per User Category.
##### STEP 4
- Oh no, the calculation seems wrong! We removed FitBit User ID from the visualization but didn’t INCLUDE that dimension in the calculation. 
- Let’s press the Undo (CTRL+Z) button.
- Adapt both measures by editing them in the field list: in each, add FitBit User ID as a second INCLUDE dimension, Syntax is {INCLUDE Dim1, Dim2 : aggregation}.
- Your visualization will not change as FitBit User ID is still in the Rows.
##### STEP 5
- Let’s now try again and remove FitBit User ID from the Rows.
- Tadaa! We now see the averages for both measures, per User Category.


#### Exercise question:
Individuals of which User Category have the highest average Heart Rate per Hour? Provide the name of User Category.

#### End goal:

<img width="298" alt="image" src="https://user-images.githubusercontent.com/95186405/145714254-d95b5d82-0247-4e85-82e1-e06cb8ed7777.png">

