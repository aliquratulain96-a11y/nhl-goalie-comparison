# nhl-goalie-comparison
An R-based analysis comparing expected and actual goals allowed among NHL goalies using MoneyPuck data.
# NHL Goalie Comparison: Expected vs Actual Goals Allowed

## Project Overview

This project explores NHL goaltender performance by comparing expected goals against with actual goals allowed. Using goalie-level data from MoneyPuck, the analysis visualizes how actual goals allowed compare with expected goals allowed for the goalies included in the dataset.

The project uses R and `ggplot2` to create a scatter plot that makes differences between expected and actual outcomes easier to examine.

## Research Question

How do actual goals allowed compare with expected goals allowed among the NHL goalies included in the analysis?

## Data

The analysis uses NHL goalie data downloaded from MoneyPuck. The dataset includes goalie identifiers, names, teams, playing time, expected goals, and actual goals, alongside other statistical measures.

The chart uses the `xgoals` and `goals` fields from the dataset. The records included in the analysis depend on the filtering applied during data preparation.

**Data source:** [MoneyPuck](https://moneypuck.com/data.htm)

## Methodology

The analysis was conducted using RStudio.

1. Imported the goalie data from a CSV file.
2. Selected the relevant fields for goalie names, expected goals, and actual goals.
3. Removed records with missing values in the fields used for the chart.
4. Created a scatter plot comparing expected goals allowed on the horizontal axis with actual goals allowed on the vertical axis.
5. Added a diagonal reference line to distinguish observations where actual goals allowed are above or below expected goals allowed.
6. Adjusted point labels and plot formatting to improve readability.

## Understanding the Visualization

Each point represents a goalie in the analyzed dataset.

- **Expected goals allowed:** The expected-goals measure recorded in the source dataset.
- **Actual goals allowed:** The actual-goals measure recorded in the source dataset.
- **Diagonal reference line:** Represents equal expected and actual values.
- **Below the line:** Fewer actual goals allowed than expected.
- **Above the line:** More actual goals allowed than expected.

These comparisons describe outcomes relative to the expected-goals measure; they should not be interpreted as a complete assessment of a goalie's ability without considering factors such as playing time, shot quality, and the context of the observations.

## Tools Used

- R
- RStudio
- `ggplot2`
- `ggrepel`
- CSV data
- GitHub

## Project Output

The main output is a scatter plot titled **NHL Goalies: Expected vs Actual Goals Allowed**. The visualization is designed to support a straightforward comparison of expected and actual outcomes while keeping goalie labels readable.

## Limitations

The findings depend on the records and filters included in the analysis. The chart alone does not establish why a goalie performed above or below the expected-goals reference line. The interpretation also depends on the precise definitions and aggregation of the source dataset's statistical fields.

## Reproducibility

The R script and the CSV used for the visualization are included in this repository so that the analysis can be inspected and reproduced, subject to the availability and terms of the original data source.

## Author

Qurat Ul Ain Ali
