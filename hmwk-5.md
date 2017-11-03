### For 10.19.17 class
### Andrea Archer
### SIG-6170 Metrics and Data Visualization I
### [Prototype 1: Time-Series/Stats](https://github.com/sva-dsi/2017-fall-course/blob/master/syllabus.md#assignment-5)

## INTRODUCTION

_1. Find some time-series or statistical data.
2. Think about the narrative that you might build around it.
3. Write a pitch (< 3 ¶s) explaining your story and linking to the data.
4. Defend your pitch in a few short arguments, describing the format of your data, and what tools/languages you would use to explore and visualize it.
5. Use your practice exercise to defend your pitch with a prototype, or test your data with RAW._

## ANALYSIS

On the NYC Open Data portal, I found some interesting time series data on [water quality complaints](https://data.cityofnewyork.us/Environment/Water-Quality-complaints/qfe3-6dkn) recorded throughout the City since January 2010. Because I don’t have a lot of prior knowledge on city water issues (all I know is that it usually tastes v good), and because the dataset is quite large with almost 10k logged incidents, I downloaded a `.csv` and played around with visualizing the data in RAW in order to quickly see what kind of arguments I might be able to pull from the data.

And after exploring a little, I chose to present the data in a Gantt chart because not only is it important to see the number and frequency of unique water quality complaints but also how long it generally took to close those complaints. The individual complaints are grouped by community board number, which seems appropriate given that your CB would be the entity to address any long-term or significant water issues within that tract. Also, the complaints are color-coded according to borough, because if there are any larger geopolitical issues surrounding clean water, it would be helpful to see those patterns too.

At the bottom of this gist is an image of the RAW visualization because the code was crazy-long and was making my browser freeze when I tried to copy it :/

With this data I would like to argue that Staten Island is poisoning its residents’ water supply and doesn’t care. Just kidding!

There is not enough information in this dataset alone (I think; I’m no statistician) to make any compelling arguments about NYC water quality in good conscience. Yes, there is a correlation between Staten Island as a borough and its CBs having a higher quantity/frequency of complaints that sometimes take _years_ to resolve… but also Staten Island could just have whinier people. Or just a lot _more_ people per community board. Or perhaps people in the Bronx, for example, are less motivated by/connected to their public services… or maybe some of the really prolonged issues are just glitches in the data… WHO KNOWS.

_Note: with a little more time I would also probably clean up this visualization a bit, for example, by grouping all the community boards within the same borough together and ordering them numerically so it’s more clear/intuitive. I would also use the addresses in the dataset to resolve the “unspecified” community boards or just delete them because they add confusion and clutter to the viz. I also want to acknowledge that my Gantt charts looks kind of like Hebrew writing… which would be awesome if it connected to my story somehow, but it doesn’t. :(_

![NYC Water Viz](https://github.com/aharcher/gh-demo/blob/master/imgs/water.png)
