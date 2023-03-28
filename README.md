# Exploratory-Data-Analysis-Report

EDA report is exploring a dataset of sports activities performed by different users of a sports tracker during January and February 2021.

Data overview:
● There are 1000 records
● There are 10 attributes (columns)
● Missing values: 270 missing values in column ’location’


Findings:
1. Demographics
The graph below explores the age and proportion of male and female users.
We can see that most of them are above 15 and under 50 years old.
Most of the users are between 20 and 30 years old and most of them are women.

2. Distance: run or ride
There are two types of activities in the ‘activity’ column: running and riding a bike.
Both of them are almost equally presented in the data.
The violin plot below shows that runners’ workouts are no longer than 20 km, while
bikers naturally can go much further – up to 80 km.

3. Duration error
When looking at the column ‘duration’ one can see that there is clearly an error in the
data (see the graph ‘before’ below). The reason for that is that the timing for riders is recorded in hours, but for runners in
minutes. In order to harmonize this data, the riding times were converted into minutes
– the graph ‘after’ shows the corrected data. The scatterplot below shows the relation between duration (min) and distance (km)
for all activities – riders’ activities are more varied in terms of time and distance, while
most runners exercise for about 60 minutes maximum and don’t do more than 20 km.

4. Date error
Another anomaly has revealed itself, when trying to explore some patterns in the
‘date’ column by splitting it into days, months and years. This column’s type is ‘object’
and when trying to convert it into a ‘datatype’ it has triggered an error – format was
not matching. Looking at a sample of the data, we can see that all dates are normally
presented in day/month/year format. However, in some cases there is a 13th, 15th, 20th month and so on, which is
impossible, therefore most likely all January dates are inverted and presented in
month/day/year format.

5. Location: null values and top countries
When we group all the data in the column ‘location’, we can see that there are 270
missing values. If we visualise this data and split by type of activity, we can see that most runners are
from Kenya and most riders are from the Netherlands.
