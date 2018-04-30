code: books-dataset-example
title: Books Dataset Example
--- |

    Let's consider the following dataset:

    | Country | Region | Happiness Rank | Happiness Score | Per Capita GDP |
    | - | - | - | - | - |
    | Switzerland	| Western Europe | 	1	| 7.587	|	1.39651	|
    | Iceland	| Western Europe |	2	| 7.561	|	1.30232	|
    | Denmark	| Western Europe	| 3	| 7.527	|	1.32548	|

    What can we say about this dataset?

    * `Country` and `Region` are `identifier` variables and they use the `nominal scale`.
    * `Happiness Rank`, `Happiness Score` and `Per Capita GDP` are `measured` variables.
    * `Happiness Rank` and `Happiness Score` are on the `ordinal scale` since Rank 1 is more than Rank 2 but the difference between 1 and 2 is not the same as between 2 and 3. Ditto for `Happiness Score`.
    * `Per Capita GDP` would be a good fit for `interval scale`. While GDP zero could exist but it's similar to temperature value being zero. It does not mean that temperature (or GDP in this case) is not present.
