code: deals-dataset-example
title: Deals Dataset Example
--- |

    Consider the following dataset:

    | retailer   | date       | thumbsup | comments | title |
    |--- |--- |--- |--- |
    | Sam's Club | 2018-01-17 | 5      | 6        | 2 pk 32 oz. Vacuum Insulated Stainless Steel Water Bottle for $6.81 + Shipping $0.99 |
    | Groupon    | 2018-01-17 | 9      | 4        | NEW Sony XB30 Portable Wireless Speaker with Bluetooth, Black (2017 model) +FREE Shipping $79.99 |
    | Amazon     | 2018-01-17 | 15     | 15       | Community the Complete Series on DVD $60 lowest price ever on amazon.com |

    What statements can we make about this dataset?

    * The dataset has 3 observations for 5 variables.
    * `retailer` and `date` are good candidates for being `identifier` variables.
    * `thumbsup` and `comments` are good candidates to be `measured` variables.
    * `title` is unstructured data and we have to do some work to further extract the variables out of it. Some of the potential variables that come out of `title` are: shipping charges, price, item name, urgency in call to action etc.

    Apart from these, let's also examine the scale types for these variables:

    * `retailer` is a clear example of `nominal scale`.
    * `date` can get hard to classify. Time in general is a continuous numeric. However, we always use discrete values of time. Having said that, in this context, `date` is being used as an `enum` (aka `categorical nominal`). Even within being `categorical`, date has a sense of order to it, so, it may seem `categorical ordinal` but 2018-01-02 is not really more than 2018-01-01. It just comes afterwards. So, the best classification of `date` scale variable would be `nominal`.
    * `thumbsup` and `comments` are clearly good for `ratio` scale.
    * `title` is unstructured data. We need to extract the actual variables before we can classify them.
