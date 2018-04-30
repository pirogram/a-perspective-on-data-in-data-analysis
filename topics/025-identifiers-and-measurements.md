code: identifiers-and-measurements
title: Identifiers and Measurements
--- |

    Let's continue building on our line of thought: data is a set of observations about the values of some variables. We'll now enhance our vocabulary beyond variables and observations.

    Let's relook at the one of our simple datasets:

    | city          | max_temp | min_temp |
    |---------------|----------|----------|
    | San Francisco | 105      | 25       |
    | San Diego     | 125      | 40       |
    | Los Angeles   | 115      | 35       |
    | Santa Barbara | 112      | 33       |
    | San Jose      | 110      | 30       |

    In this dataset, `city`, `max_temp` and `min_temp` are variables. `('San Francisco', 105, 25)` is one of the observations. `('San Diego', 125, 40)` is another one. Each column represents a variable while each row represents an observation.

    While `city`, `max_temp` and `min_temp` are all variables, there is a difference among them. `max_temp` and `min_temp` are actual measurements while `city` is an identifier for specific measurements. For example, `San Francisco` identifies `(105, 25)` measurements for `max_temp` and `min_temp`. Similarly, `San Diego` identifies `(125, 40)` measurements. Extending this line of thought, we can classify `city` as an _identifier variable_ and `max_temp` & `min_temp` as _measured variables_.

    Let's apply the same framework to another dataset:

    | city          | date       | max_temp | min_temp |
    |---------------|------------|----------|----------|
    | San Francisco | 2017-01-01 | 105      | 25       |
    | San Diego     | 2017-01-01 | 135      | 50       |
    | Los Angeles   | 2017-01-01 | 125      | 45       |
    | San Francisco | 2017-01-02 | 105      | 25       |
    | San Diego     | 2017-01-02 | 135      | 50       |
    | Los Angeles   | 2017-01-02 | 125      | 45       |

    In this dataset, `city` & `date` are _identifier variables_ since together they identify a set of measurements. `max_temp` & `min_temp` are _measured variables_ since their value is being measured.

    It is important to note that `identifier` and `measured` variables are just a way of looking at data (i.e. a way of thinking about it). There are no hard and fast rules. In fact, depending on the analysis you wish to perform (or the question that you wish to answer), the classification of `identifier` and `measured` variables can change.

    Finally, even though this classification is not definitive (and varies based on the situation), it's an extremely important way of looking at the data. Tidy data is usually the one where `identifier` and `measured` variables have been separated and neatly arranged. Just look at the following couple of ways to arrange our temperature data and assess which one is easier to read and more suited for analytical queries.

    **Example 1:**

    | city          | max_temp | min_temp |
    |---------------|----------|----------|
    | San Francisco | 105      | 25       |
    | San Diego     | 125      | 40       |
    | Los Angeles   | 115      | 35       |
    | Santa Barbara | 112      | 33       |
    | San Jose      | 110      | 30       |

    **Example 2:**

    | max_temp | min_temp | city          |
    |----------|----------|---------------|
    | 105      | 25       | San Francisco |
    | 135      | 50       | San Diego     |
    | 125      | 45       | Los Angeles   |
    | 105      | 25       | San Francisco |
    | 135      | 50       | San Diego     |
    | 125      | 45       | Los Angeles   |
