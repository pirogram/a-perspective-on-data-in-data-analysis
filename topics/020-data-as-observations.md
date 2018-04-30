title: Data As Observations
code: data-as-observations
--- |
    Let's start with a few examples of how an application developer looks at data as Entities, Relationships and their Attributes:

    1. **Weather:** `city` is an entity and `max_temp` and `min_temp` are attributes of that entity.
    1. **Tweet:** `User` is an entity with `name`, `handle` as attributes. `User` publishes `Tweet` entities which have `timestamp` and `text` as attributes. A `Tweet` entity can mention one or more `User` entities.

    However, as we just discussed, an analyst looks at data as a set of observations. What are the variables in my data? What are the sets of values for those variables? Each value set is an observation. Let's look at a few examples to understand this better.

    Following hypothetical dataset has the max and min temperatures for a few cities on a specific day. In the language of data analysis, we have five observations about three variables. The variables being `city`, `max_temp` and `min_temp`.

    | city          | max_temp | min_temp |
    |---------------|----------|----------|
    | San Francisco | 105      | 25       |
    | San Diego     | 125      | 40       |
    | Los Angeles   | 115      | 35       |
    | Santa Barbara | 112      | 33       |
    | San Jose      | 110      | 30       |

    The following example is similar except that we now have six observations about four variables: `city`, `date`, `max_temp` and `min_temp`.

    | city          | date       | max_temp | min_temp |
    |---------------|------------|----------|----------|
    | San Francisco | 2017-01-01 | 105      | 25       |
    | San Diego     | 2017-01-01 | 135      | 50       |
    | Los Angeles   | 2017-01-01 | 125      | 45       |
    | San Francisco | 2017-01-02 | 105      | 25       |
    | San Diego     | 2017-01-02 | 135      | 50       |
    | Los Angeles   | 2017-01-02 | 125      | 45       |

    Let's look at some tweets related dataset. The following dataset has three observations about four variables. The variables are `name`, `handle`, `date`, `text`.

    | name               | handle         | date       | text |
    |--- |--- |--- |
    | Computer Science   | CompSciFact    | 2018-01-17 | Generating primes in Conway's Game of Life http://www.nathanieljohnston.com/2009/08/generating-sequences-of-primes-in-conways-game-of-life/ |
    | I Am Developer     | iamdeveloper   | 2018-01-17 | my favourite thing about standing desks, they keep me on my toes |
    | Srinath Srininvasa | srinaths       | 2018-01-17 | Deep learning is so yesterday, let's talk deep happiness :) |

    Here is another dataset about deals. This one has three observations about five variables (`retailer`, `date`, `rating`, `comments`, `title`).

    | retailer   | date       | rating | comments | title |
    |--- |--- |--- |--- |
    | Sam's Club | 2018-01-17 | 5      | 6        | 2 pk 32 oz. Vacuum Insulated Stainless Steel Water Bottle for $6.81 + Shipping $0.99 |
    | Groupon    | 2018-01-17 | 9      | 4        | NEW Sony XB30 Portable Wireless Speaker with Bluetooth, Black (2017 model) +FREE Shipping $79.99 |
    | Amazon     | 2018-01-17 | 15     | 15       | Community the Complete Series on DVD $60 lowest price ever on amazon.com |

    So far, we looked at the tabular representation of observations. In a tabular representation, each column represents a variable while each row is an observation.
