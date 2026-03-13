# Unit 1: Exploring One-Variable Data
> Exam Weight: 15–23% | ~14–16 Class Periods

## Topics

### 1.1 Introducing Statistics: What Can We Learn from Data?
- **Learning Objective (DAT-1.A):** Identify the question to be answered, considering the data to be collected or already available
- **Essential Knowledge:**
  - Statistics is the science of learning from data
  - Data analysis begins with a clear question or problem
  - Individuals are the objects described by a set of data; a variable is any characteristic of an individual

### 1.2 The Language of Variation: Variables
- **Learning Objective (VAR-1.A):** Identify variables as categorical or quantitative
- **Essential Knowledge:**
  - A **categorical variable** assigns labels or group names (e.g., color, gender, zip code)
  - A **quantitative variable** takes numerical values for which arithmetic operations make sense (e.g., height, income)
  - Quantitative variables can be discrete (countable) or continuous (measurable)

### 1.3 Representing a Categorical Variable with Tables
- **Learning Objective (UNC-1.A):** Represent categorical data using frequency or relative frequency tables
- **Essential Knowledge:**
  - A **frequency table** gives the count of observations in each category
  - A **relative frequency table** gives the proportion (or percentage) of observations in each category
  - Relative frequency = $\frac{\text{frequency}}{\text{total count}}$

### 1.4 Representing a Categorical Variable with Graphs
- **Learning Objective (UNC-1.B):** Represent categorical data using bar charts and pie charts
- **Essential Knowledge:**
  - **Bar charts** display the distribution of a categorical variable; bars have gaps between them
  - Bar charts can show frequency or relative frequency
  - **Pie charts** show parts of a whole (require categories to sum to 100%)
  - Bar charts are generally preferred over pie charts for comparisons

### 1.5 Representing a Quantitative Variable with Graphs
- **Learning Objective (UNC-1.C):** Represent quantitative data using dotplots, histograms, and stemplots
- **Essential Knowledge:**
  - **Dotplots** place a dot for each observation above the number line
  - **Histograms** group data into bins (intervals) and display frequencies or relative frequencies
  - **Stemplots** (stem-and-leaf plots) separate each value into a stem and leaf
  - The choice of bin width in histograms affects the appearance of the distribution

### 1.6 Describing the Distribution of a Quantitative Variable
- **Learning Objective (UNC-1.D):** Describe the shape, center, and variability of a distribution
- **Essential Knowledge:**
  - **Shape:** symmetric, skewed left, skewed right, unimodal, bimodal, uniform
  - **Center:** where the "middle" of the data lies (mean or median)
  - **Spread (variability):** how spread out the data are (range, IQR, standard deviation)
  - **Unusual features:** outliers, gaps, clusters
  - Always describe distributions in **context** (referring to the variable)

### 1.7 Summary Statistics for a Quantitative Variable
- **Learning Objective (UNC-1.E):** Calculate and interpret summary statistics
- **Essential Knowledge:**
  - **Mean:** $\bar{x} = \frac{1}{n} \sum_{i=1}^{n} x_i$ — the arithmetic average; sensitive to outliers
  - **Median:** the middle value when data are ordered; resistant to outliers
  - **Quartiles:** $Q_1$ (25th percentile), $Q_3$ (75th percentile)
  - **IQR:** $Q_3 - Q_1$ — measures the spread of the middle 50%
  - **Standard deviation:** $s = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n - 1}}$ — measures typical distance from the mean
  - **Variance:** $s^2 = \frac{\sum (x_i - \bar{x})^2}{n - 1}$
  - For skewed distributions, median and IQR are more appropriate than mean and standard deviation

### 1.8 Graphical Representations of Summary Statistics
- **Learning Objective (UNC-1.F):** Represent summary statistics graphically using boxplots
- **Essential Knowledge:**
  - **Five-number summary:** minimum, $Q_1$, median, $Q_3$, maximum
  - **Boxplot:** graphical display of the five-number summary
  - **Modified boxplot:** marks outliers individually; whiskers extend to the most extreme non-outlier values
  - Outlier rule: a value is an outlier if it falls more than $1.5 \cdot IQR$ below $Q_1$ or above $Q_3$

### 1.9 Comparing Distributions of a Quantitative Variable
- **Learning Objective (DAT-1.B):** Compare distributions of quantitative data using back-to-back stemplots, parallel dotplots, or side-by-side boxplots
- **Essential Knowledge:**
  - When comparing distributions, address **shape**, **center**, **spread**, and **unusual features** for each group
  - Use comparative language: "Group A has a higher median than Group B"
  - Side-by-side boxplots and back-to-back stemplots facilitate direct comparison

### 1.10 The Normal Distribution
- **Learning Objective (VAR-2.A):** Calculate and interpret z-scores; use the normal distribution to find proportions
- **Essential Knowledge:**
  - The **normal distribution** is symmetric, bell-shaped, and described by mean $\mu$ and standard deviation $\sigma$: $N(\mu, \sigma)$
  - **z-score:** $z = \frac{x - \mu}{\sigma}$ — the number of standard deviations a value is from the mean
  - **Empirical Rule (68-95-99.7):** Approximately 68% of data fall within 1 SD, 95% within 2 SD, 99.7% within 3 SD of the mean
  - Use the **standard normal table** or calculator (normalcdf, invNorm) to find areas/proportions
  - A normal probability plot (Q-Q plot) can assess whether data follow a normal distribution

## Common Misconceptions
- Confusing bar charts (categorical) with histograms (quantitative) — histograms have no gaps between bars
- Thinking the mean is always the best measure of center — median is preferred for skewed data
- Forgetting to describe distributions in context
- Confusing "standard deviation" with "standard error" (Unit 5+)
- Assuming all data are normally distributed
