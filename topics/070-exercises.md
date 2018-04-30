code: exercises
title: Exercises
---
type: multiple-choice-question
id: 1
question: |
  What statements are true about the following dataset:

  ```
  student,height
  Ram,4.2
  Shyam,5.1
  George,5.0
  Rachel,4.8
  ```
options:
  - text: It has 2 observations and 4 variables.
  - text: It has 4 observations and 2 variables.
    correct: true
  - text: |
      `student` is an `identifier` variable and `height` is a `measured` variable.
    correct: true
  - text: |
      `student` uses `ordinal` scale.

---

type: categorization-question
id: 2
question: |
  Categorize the variables from the following dataset into their scale.

  | retailer   | date       | thumbsup | comments | title |
  |--- |--- |--- |--- |
  | Sam's Club | 2018-01-17 | 5      | 6        | 2 pk 32 oz. Vacuum Insulated Stainless Steel Water Bottle for $6.81 + Shipping $0.99 |
  | Groupon    | 2018-01-17 | 9      | 4        | NEW Sony XB30 Portable Wireless Speaker with Bluetooth, Black (2017 model) +FREE Shipping $79.99 |
  | Amazon     | 2018-01-17 | 15     | 15       | Community the Complete Series on DVD $60 lowest price ever on amazon.com |

categories: ['nominal', 'ordinal', 'interval', 'ratio', 'unstructured']
mappings:
  retailer: nominal
  date: nominal
  thumbsup: ratio
  comments: ratio
  title: unstructured
help: |
  Categorization of `date` (or time in general) could be tricky. It partially matches the criteria for `nominal`, `ordinal` as well as `interval`. In the context of this dataset, `categorical nominal` seems the closest match. However, there is room for debate on this one.

  This also goes to show that these categorizations are not precise but more as a framework for thinking.

---

type: categorization-question
id: 3
question: |
  Categorize the variables from the following dataset into `identifier` and `measured` categories.

  | retailer   | date       | thumbsup | comments | title |
  |--- |--- |--- |--- |
  | Sam's Club | 2018-01-17 | 5      | 6        | 2 pk 32 oz. Vacuum Insulated Stainless Steel Water Bottle for $6.81 + Shipping $0.99 |
  | Groupon    | 2018-01-17 | 9      | 4        | NEW Sony XB30 Portable Wireless Speaker with Bluetooth, Black (2017 model) +FREE Shipping $79.99 |
  | Amazon     | 2018-01-17 | 15     | 15       | Community the Complete Series on DVD $60 lowest price ever on amazon.com |

categories: ['identifier', 'measured']
mappings:
  retailer: identifier
  date: identifier
  thumbsup: measured
  comments: measured
  title: measured