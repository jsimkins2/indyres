
# Final Project: World Cup Data

<br> <br>
<img src="images/soccer.jpg" width="70%" style="display: block; margin: auto;" />
<br> <br>

In this final comprehension check, we’ll utilize skills we’ve learned
over the past 4 days to investigate FIFA World Cup data. The World Cup
is the most popular single-sport contest in the world, watched by over
3.5 billion people around the world. Every 4 years, the top 32 countries
join to compete in this exciting soccer tournament. The best players on
the planet show off their skills and teamwork in an attempt to capture
the most sought after prize in sport - the FIFA World Cup Trophy.

## About the Data

This dataset contains information regarding the total television
audience for the 2010 World cup. Before proceeding, download the
`fifa_audience_2010.xlxs` file from the course datasets
folder.

| Variable             | Definition                                                                                                                                                                                                                    |
| :------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| country              | The name of the country audience                                                                                                                                                                                              |
| confederation        | Each country is a member of a regional soccer organization called a confederation. For example, the United States are part of CONCACAF, which is comprised of North American countries such as Mexico, Canada, Honduras, etc. |
| population\_share    | The relative percentage of world population share                                                                                                                                                                             |
| tv\_audience\_share  | The relative percentage of television audience                                                                                                                                                                                |
| gdp\_weighted\_share | The relative percentage of gross domestic product (purchasing power) per country                                                                                                                                              |

## Assessment

The final assessment requires the submission of an R script. It is worth
25 points. Your script will be graded based on the following:
<br>

| Value     | Grading Metric                                                                                |
| :-------- | :-------------------------------------------------------------------------------------------- |
| 15 points | Ability to accomplish 5 coding tasks listed below                                             |
| 5 points  | Methodology and discussion of what’s being attempted in each coding task                      |
| 5 points  | Organization of R script (where packages are loaded, where data is read in, commenting, etc.) |

<br>

### Coding Tasks

1.  Load appropriate packages, then load in the
    `fifa_audience_2010.xlxs` file. Answer the following via coding.
      - Convert this from a tibble dataframe to a standard dataframe.
      - What are the dimensions of the dataframe?
      - What are the column names?
      - What is the class of the country variable?
      - What country is located in the 15th row?
      - What is the class of the 15th country? (just the country itself)
        <br> <br>
2.  Sort the dataframe based on the population\_share (from highest
    share to lowest share). Answer the following via coding.
      - What country is 10th in popoulation share?
      - How many countries have a rounded relative population\_share of
        0.0%?
      - The `cor()` function calculates the correlation between two
        vectors. A perfect match has a correlation of 1 and complete
        opposites have a correlation value of 0. What is the correlation
        between `gdp_weighted_share` and `population_share`. Does it
        make sense? <br> <br>
3.  Create a scatter plot of `gdp_weighted_share` and
    `population_share`. Include the following
      - Colors, x label, y label, and a `pch` value of 21
      - Include the correlation value calculated above in your title
        <br> <br>
4.  Create a bar plot of the `population share` of *the top 10
    countries* based on this variable.
      - Use the `barplot()` function. (hint:use `help(barplot)` if
        you’re stuck)
      - Include colors, x label, y label, title <br> <br>
5.  Create a pie chart of the various confederations.
      - Include percentages and percentage symbol
      - Include unique colors, title, and labels
