code: data-labels
title: Data Labels
--- |

    Let's revisit our sample dataset of day wise observations of max and min temperatures for a few cities. As we discussed so far, this date has 6 observations about 4 variables. The `identifier` variables are `city` and `date`. The `measured` variables are `max_temp` and `min_temp`.

    | city          | date       | max_temp | min_temp |
    |---------------|------------|----------|----------|
    | San Francisco | 2017-01-01 | 105      | 25       |
    | San Diego     | 2017-01-01 | 135      | 50       |
    | Los Angeles   | 2017-01-01 | 125      | 45       |
    | San Francisco | 2017-01-02 | 105      | 33       |
    | San Diego     | 2017-01-02 | 135      | 50       |
    | Los Angeles   | 2017-01-02 | 125      | 45       |

    Purely from a tabular data representation perspective, we can look at `city`, `date`, `max_temp` and `min_temp` as labels on columns. On the other hand, each row could be seen as a composition of two types of values:
    * the city name & date values (e.g. `('San Francisco', '2017-01-01')` and `('San Francisco', '2017-01-02')`) can be seen as labels on rows.
    * the max_temp and min_temp values (e.g. `(105, 25)`, `(105, 33)`) can be seen as measurements.

    This way of looking at data is very different from the RDBMS way of looking at the data. In the relational database land, we have the mental model of columns being labeled but we do not have the mental model of rows being composed of labels and measurements. In the context of data analysis, it's often helpful to think in terms of row values as labels and measurements since that helps us separate the identifiers of an observation from the measurements of an observation.

    Again, it's not always possible to cleanly demarcate labels and measurements in the context of an observation (aka row of data). However, it's an important mental model that goes a long way in reasoning about the dataset.
