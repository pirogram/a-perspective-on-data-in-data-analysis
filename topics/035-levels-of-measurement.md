code: levels-of-measurement
title: Levels of Measurement
--- |

    Application developers are all too familiar with data types of their variables. A variable could be a `char`, `int`, `float` etc. It could get more granular with `uint8`, `float64` etc. In object oriented languages, we can define our own data types (kind of) by saying that a variable could be of `Car` data type.

    One of the important aspect of these data types is that different data types allow us to perform different types of operations on the variable. For example, we cannot perform mathematical operations on `char`, we can divide an `uint8` by another `unit8` but we cannot assign it a negative value or a floating point value.

    Similarly, in the field of data analysis, variables have an analogous of data type. This _analogous of data type_ goes by the names of _scale of measurement_ or _levels of measurement_. In this section, we'll go over them and develop an intuition about them.

    ## Nominal (Scale)

    A `Nominal Scale` broadly maps to `enum` data type in programming. The values in a nominal scale cannot be compared with each other. They are just distinct values. For example, names of people or other entities, days of the week, color of eyes, fruit names etc. These are all examples of variables that use `Nominal Scale` and hence are called `nominal` variables.

    When we are dealing with `nominal` variables, we can only count the instances of different values and look at the percentage distribution. We cannot average them or even arrange them in a particular order (because there is no sense of ordering here).

    ## Ordinal (Scale)

    `Ordinal Scale` is like `Nominal Scale` with the difference that the distinct values on `Ordinal Scale` have an order. One value is more than the other. For example, five point rating system on Amazon where rating 5 is more than rating 4. Similarly, happiness level of different communities where "Ecstatic" is more than "Happy".

    One could argue that days of week form Ordinal Scale and not Nominal Scale since there is a sense of ordering within days of week (Tue comes after Mon). However, since we cannot say that Tue is _more_ than Mon, the days of week go on the Nominal Scale.

    Since, Ordinal variables have a sense of more (or less), we could say that rating 5 is more than rating 4 and do a comparison between different rating values. However, computing averages is still a misleading piece of information. Since the difference between rating 3 and 4 is not same as rating 4 and 5, computing the average rating only provides a subjective sense. There is definitive meaning of average rating 3. Also, we cannot say that two items with the same average rating are expected to provide equal satisfaction.

    ## Interval (Scale)

    `Interval Scale` is like `Ordinal Scale` with the additional property that interval between values has the same meaning. For temperature, difference between 60F and 70F is same as 70F and 80F. Of course, it's not the same in the overall effect on environment but it's the same from the physical characteristics point of view.

    `Interval Scale` maps to variables that do not have a zero value. Temperature is one of them. 0 degree F is not absence of temperature. Another example would be IQ score. It has a notion of interval but do we have a notion of 0 value in IQ score?


    ## Ratio (Scale)

    `Ratio Scale` is like `Interval Scale` with the additional property that it could be 0. Most of the numeric variables (whether discrete or continuous) fall on the `Ratio Scale`. Examples are house prices, number of emails in mailbox, miles traveled etc.

    ## Un-Scale

    Other than the aforementioned (which are classic textbookish scales), there are some variables that deserve a special mention. Either you cannot apply a scale to these variables or the scale you choose would depend on the context.

    * **Time:** Any variable that represents date or time falls in this category. Presence of time variable in the dataset often leads us in specific directions of analysis that we would not take otherwise.
    * **Unstructured:** This is hugely important. Some of the variables may have unstructured data (e.g. text of a Tweet or a Facebook post). We usually deal with this kind of variables by deriving other variables out of it (e.g. sentiment score, length etc).
    * **Perceptual:** In the field of machine learning, we also deal with variables that can be classified as perceptual. Voice, Images, Videos etc fall in this category. At times, we treat them as unstructured data (i.e. extract other variables out of them) and some times, they are fed "as is" into machine learning algorithms.
