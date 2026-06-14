# Unit 1: Exploring One-Variable Data
> Exam Weight: 15–23% | ~14–16 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content now in **new Unit 1** (the normal distribution moved to new Unit 2 as a probability model). See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 1.1 What Statistics Is About
Statistics turns data into knowledge by working through a cycle: pose a question, gather data, analyze, and interpret. Every investigation begins with understanding what question the data should answer.
- Individuals are the objects described in a dataset; a variable is any characteristic measured for each individual
- Distinguishing what is being measured — and for whom — guides every analytical choice that follows

### 1.2 Types of Variables
How a variable can be measured determines which summaries and graphs are appropriate.
- A **categorical variable** places each individual into a group or label (e.g., color, major, yes/no response)
- A **quantitative variable** records a number for which arithmetic comparisons make sense (e.g., height, temperature)
- Quantitative variables are discrete (countable whole numbers) or continuous (measured on a scale with no gaps)

### 1.3 Frequency and Relative Frequency Tables for Categorical Data
The simplest categorical summary counts how often each group appears.
- A **frequency table** records the count per category
- A **relative frequency table** expresses each count as a proportion: $\text{relative frequency} = \frac{\text{count}}{\text{total}}$

### 1.4 Graphing Categorical Data
Graphs give a quick visual overview of how a categorical variable is distributed.
- **Bar charts** display counts or proportions with one bar per category; gaps between bars show these are distinct groups
- **Pie charts** represent each category as a share of a whole; all slices must sum to 100%
- Bar charts generally make comparisons across categories easier to read than pie charts

### 1.5 Graphing Quantitative Data
Several graph types reveal a quantitative distribution from different angles.
- **Dotplots** place a dot above the number line for each observation; useful for small datasets
- **Histograms** sort data into equal-width bins and display frequency or relative frequency per bin; bin width shapes how the distribution appears
- **Stemplots** (stem-and-leaf plots) split each value into a stem and leaf, preserving individual data values while showing shape

### 1.6 Describing a Distribution
A complete description of a quantitative distribution addresses four features, always in context.
- **Shape:** symmetric, skewed left (long tail toward smaller values), skewed right (long tail toward larger values), unimodal, bimodal, uniform
- **Center:** where the data cluster — the "typical" value, measured by mean or median
- **Spread:** how dispersed the values are — range, IQR, or standard deviation
- **Unusual features:** outliers, gaps, clusters — anything that breaks the general pattern
- Always name the variable when describing its distribution; "the data are right-skewed" is incomplete without context

### 1.7 Numerical Summary Statistics
A small set of numbers can capture the essential shape of a distribution.
- **Mean:** $\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i$ — the arithmetic average; pulled toward extreme values
- **Median:** the middle value when data are sorted; not influenced by outliers
- **Quartiles:** $Q_1$ (25th percentile) and $Q_3$ (75th percentile)
- **IQR:** $Q_3 - Q_1$ — the spread of the middle 50% of data
- **Standard deviation:** $s = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n - 1}}$ — average distance from the mean
- **Variance:** $s^2 = \frac{\sum (x_i - \bar{x})^2}{n - 1}$
- When a distribution is skewed, the median and IQR are more informative than the mean and standard deviation

### 1.8 Boxplots
A boxplot translates the five-number summary into a visual display.
- **Five-number summary:** minimum, $Q_1$, median, $Q_3$, maximum
- **Modified boxplot:** outliers are plotted as individual points; whiskers reach the most extreme non-outlier values
- Outlier identification rule: values more than $1.5 \cdot IQR$ below $Q_1$ or above $Q_3$ are marked as outliers

### 1.9 Comparing Distributions
Side-by-side boxplots, parallel dotplots, and back-to-back stemplots allow direct comparison across groups.
- Address shape, center, spread, and unusual features for each group being compared
- Use comparative language in context: "the median house price in Group A is higher than in Group B"

### 1.10 The Normal Distribution
The normal distribution is a symmetric, bell-shaped probability model that arises naturally in many real-world settings.
- Described by mean $\mu$ and standard deviation $\sigma$: $N(\mu, \sigma)$
- **z-score:** $z = \frac{x - \mu}{\sigma}$ — the number of standard deviations a value sits above or below the mean
- **Empirical (68-95-99.7) Rule:** approximately 68% of values fall within 1 SD, 95% within 2 SD, and 99.7% within 3 SD of the mean
- Normal probabilities and inverse values are found with a calculator (normalcdf, invNorm) or a standard normal table
- A normal probability plot (Q-Q plot) helps assess whether a dataset is well-described by a normal model

## Common Misconceptions
- Histograms and bar charts look similar but serve different purposes — histogram bars touch (continuous intervals), bar chart bars have gaps (distinct categories)
- The mean is not always the best center measure — it is pulled by skewness and outliers, making the median more appropriate in such cases
- Distribution descriptions must reference the variable and its context, not just say "the data are right-skewed"
- "Standard deviation" and "standard error" are different concepts; standard error describes how a statistic varies across samples (covered in Unit 5 and beyond)
- Normality should not be assumed — it must be verified from graphs or probability plots
