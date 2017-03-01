### Summary

The dataset I'm using is Titanic.csv. My conclusion is "Peopole in higher class tends to survive more". In my viusalization, I made a bar chart for the overall survival rate grouped by the class. Class 1(High class) has much higher survival rate than class 2(Mid class) and class 3 (Low class), and the amount of survived people from High class is even higher than from Low class though the total amounts of High class passengers are much lower.

### Design

Initial design: By explortary data analysis using ipython, I found that the survival rate differs in different class, and also in age and sex. So i grouped the data with different class(High/Mid/Low), then group the people by thier age to Child(age<12), elders(>65) and others. For this data set there are 177 empty value for Age group. Considering the average age value for the whole dataset is almost 30 which is neither "child" nor "elder", I decide to put the empty value into the "Others" group. 

After this i then export the data to a new csv called "Titan.csv" and load it into the index.html file and use Dimple.js. With the Index.html file, i first create SVG element as the canvas for the chart, then with the loaded data, I binded the data with the 'body' element and draw the "bar" for each data point with Dimple.js, then I used button.on to update the active option to visualize the data by each different group method. 

For the chart itself, there are three different charts: "Overview", "Agegroup" and "Sex". In order to see the overall survival rate for each class, I created the "Overview". While age is also an important feature for the survival rate, i then grouped further to "Class/Agegroup", while the Agegroup includes "Child (age<12)", "Elders (age>65)" and "Others". Meanwhile "sex" is another important feature so i added "sex" to group the passengers based on their Genders.
By clicking the different buttons we shall find the different chart with different group methods.

##### Deedback 1: 

What do you notice in the visualization?
The colors and the theme are tied together very well. The visualization feels complete. The colors are light on the eyes, and you did a good job on using pastels.

What questions do you have about the data?
If I wasn't well versed in the Titanic data, I would not have known what the Pclass numbers meant. I would suggest perhaps labelling which one is upper class, middle, and lower to enhance comprehension for the view.

What relationships do you notice?
I definitely notice important trends right away, such as more passengers dying than surviving. I also am able to see also that men died more than women.

What do you think is the main takeaway from this visualization? 
That there is more detail to the Titanic passenger data than who died and who survived. The visualization dives into the finer details and does a good job.

Is there something you don’t understand in the graphics?
I liked that the x-axis changed with each button, however it was confusing to see two unique variables on one axis. I would suggest only to implement one name.


##### Feedback 2: 
可以注意到不同条件下存活率的差异和不同组别的人数。
可以把数据的背景简单介绍一下，比如数据的总人数，是乘客还是船员，还是都有？
我觉得主要表达的是 不同条件下存活率的差异。（但是你的纵坐标是count，重心容易放到人数的分布上）
可以改进的地方：
无法直观的看到存活率，建议添加数字。最好能够把纵轴改为存活率。

##### Feedback 3:
In your description paragraph, you mention ...in the Titanic disaster except Rose?
Although Titanic is a popular movie, not everyone may have seen it or recall who Rose is. You can refresh their memory by maybe adding a hyperlink to Rose's IMDB page:
...in the Titanic disaster except [Rose](http://www.imdb.com/character/ch0002339/bio)?

In my opinion the legend is not lined up with your chart. You can clean this up by moving your legend a bit to the left, and moving your buttons a bit down so that it is in line with your chart and looks neat.

I would also suggest you change your x Axis title to be more descriptive (rather than the default name). For example, change "Pclass" -> "Passenger Class".

### Design after Feedback
- Used PctAxis as the y axis, so that it shows more clear information about the survival rate. And added the amount of passengers for each group, so that the reader can have an idea of how big is the group when I talk about the survival rate. 
- Changed the labels of x-axis as "High/Mid/Low class" so that it's more clear than just using 1,2,3
- Minor corrections about the positions of the legend and buttons
- Minor corrections on the descriptions.


### Resources

##### Udacity course and its code for lesson 2 and lesson 6.
##### http://dimplejs.org
##### https://d3js.org
##### Udacity members assignment: https://edaward.github.io


