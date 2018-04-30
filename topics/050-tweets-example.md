code: tweets-dataset-example
title: Tweets Dataset Example
--- |

    Let's consider the following (hypothetical) dataset:

    | name               | handle         | date       | text | retweets | replies |
    |--- |--- |--- | --- | --- |
    | Computer Science   | CompSciFact    | 2018-01-17 | Generating primes in Conway's Game of Life http://www.nathanieljohnston.com/2009/08/generating-sequences-of-primes-in-conways-game-of-life/ | 24 | 3 |
    | I Am Developer     | iamdeveloper   | 2018-01-17 | my favourite thing about standing desks, they keep me on my toes | 49 | 12 |
    | Srinath Srininvasa | srinaths       | 2018-01-17 | Deep learning is so yesterday, let's talk deep happiness :) | 2 | 1 |

    What can we say about this dataset?

    * It has 3 observations across 6 variables.
    * `name` and `handle` are easily the `identifier` variables. In fact, `handle` is _the_ `identifier` variable here while `name` is just attached to the `handle`. We are not likely to use `name` alone as the `identifier` for observations because multiple people can share a name.
    * As usual, `date` could be used as `identifier` variable (e.g. when you want to plot the activity on time axis). It could also be a `measured` variable when you want to see which users are more active on which dates.
    * `retweets` and `replies` are clearly the measured variables.
    * `text` needs further work and different variables should be extracted from `text` for analysis purpose.

    What else can we say about the dataset?

    * `name` and `handle` use the `nominal` scale.
    * `date` in this case could be on `nominal scale` as `identifier` or `interval scale` as `measured`.
    * `retweets` and `replies` are on `ratio scale`.
    * `text` needs work.
