# Goal Analysis in Men's vs. Women's FIFA World Cup Matches

## Overview

This project investigates whether more goals are scored in women's FIFA World Cup matches compared to men's using statistical hypothesis testing. By analyzing data from official FIFA World Cup matches since 2002, we aim to provide insights into scoring trends across genders.

## Hypotheses

- **Null Hypothesis (\(H_0\))**: The mean number of goals scored in women's FIFA World Cup matches is the same as in men's.
- **Alternative Hypothesis (\(H_A\))**: The mean number of goals scored in women's FIFA World Cup matches is greater than in men's.

The analysis uses a **10% significance level**.

## Data

The analysis is based on two datasets containing the results of men's and women's international soccer matches. The datasets were filtered to include only official FIFA World Cup matches (excluding qualifiers) played after 2002-01-01.

- `men_results.csv`: Results of men's FIFA World Cup matches
- `women_results.csv`: Results of women's FIFA World Cup matches

## Methodology

1. **Data Filtering**:
   - Filtered datasets to include only official FIFA World Cup matches since 2002-01-01.

2. **Goals Calculation**:
   - Computed the total number of goals scored in each match (sum of home and away team scores).

3. **Visualization**:
   - Generated histograms to visualize the distribution of goals scored in men's and women's matches.

4. **Statistical Analysis**:
   - Applied a one-tailed Wilcoxon-Mann-Whitney test to compare the distribution of goals scored between the two groups.

5. **Interpretation**:
   - Used the p-value from the test to determine whether to reject the null hypothesis.

## Results

- **P-value**: The p-value obtained from the Wilcoxon-Mann-Whitney test (0.005106609825443641).
- **Conclusion**:
  - p-value < 0.1 : The null hypothesis was rejected, indicating that more goals are scored in women's matches.

## Dependencies

The following Python libraries were used for the analysis:

- `pandas`
- `matplotlib`
- `pingouin`

