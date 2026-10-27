# Recipe and User Review Analysis Using PySpark

## Project Overview

This project explores recipe and user-review data using **PySpark** to
understand preparation times, nutritional information, recipe tags, and
user ratings. It also demonstrates data cleaning and feature engineering
on a large dataset.

The analysis covers **231,637 recipes** and approximately **1.13 million
user reviews**.

## Objectives

-   Explore recipe preparation times and identify typical cooking
    durations.
-   Prepare nutritional attributes for more comparable analysis.
-   Check review-date consistency against recipe submission dates.
-   Examine popular recipe tags and highly rated tags.
-   Engineer time-based and user-rating features for further analysis.

## Tools and Technologies

-   **Python**
-   **Apache Spark / PySpark**
-   Jupyter Notebook
-   Data cleaning and feature engineering
-   Exploratory data analysis (EDA)

## Key Analysis Outcomes

-   **Dataset scale:** Analyzed 231,637 recipes and approximately 1.13
    million reviews.
-   **Preparation time:** The median preparation time was **40
    minutes**, providing a useful measure of a typical recipe's
    preparation duration.
-   **Review-date quality:** Identified **1,246 reviews** dated earlier
    than the corresponding recipe submission date. These were excluded
    from the analysis to improve date consistency.
-   **Nutrition analysis:** Standardized seven nutritional attributes
    per 100 calories to support more comparable nutritional analysis.
-   **Tags and ratings:** Examined 29 frequent tags and 26 highly rated
    tags, using an average-rating threshold above 4.53 and more than 100
    ratings for the highly rated group.
-   **Feature engineering:** Created time-based and user-level rating
    features, resulting in a dataset with 148 columns for further
    exploration.

## Workflow

1.  Loaded recipe and review data.
2.  Explored dataset structure and key fields.
3.  Checked preparation-time values and handled extreme durations for
    analysis.
4.  Compared review dates with recipe submission dates and excluded
    inconsistent records.
5.  Prepared nutritional features for comparison.
6.  Analyzed recipe tags and rating patterns.
7.  Created time-based and user-rating features for downstream analysis.

## Potential Applications

The findings can help inform future recipe discovery or recommendation
work by describing preparation-time patterns, nutritional attributes,
tag popularity, and rating behavior. **This project is exploratory
analysis; it does not by itself demonstrate a deployed recommendation
system or measured improvement in user engagement.**

## Repository Contents

-   `Recipe_EDA_PySpark.ipynb` --- notebook containing the analysis.
-   Dataset files --- add the required recipe and review datasets if you
    are permitted to redistribute them.

> Update the notebook filename above to match the actual file you
> upload. If the original data is subject to licensing or size
> restrictions, document where it can be obtained instead of committing
> it to GitHub.

## How to Run

1.  Clone or download this repository.
2.  Install Python, Jupyter Notebook, and PySpark in your environment.
3.  Obtain the input recipe and review datasets and place them in the
    paths expected by the notebook.
4.  Open the notebook and update file paths if necessary.
5.  Run the notebook cells in order.

Example installation command:

``` bash
pip install pyspark jupyter pandas
```

The exact dependencies may vary depending on the notebook's imports and
environment.

## Notes and Limitations

-   Reported results should be reproduced by running the notebook with
    the original datasets and environment.
-   The treatment of extreme preparation times and the date-filtering
    logic should be reviewed before using the cleaned data in a
    production workflow.
-   The analysis identifies patterns and prepares features; it does not
    establish causation or prove business impact.

## Author

**Krishna**\
Data Analytics Portfolio Project
