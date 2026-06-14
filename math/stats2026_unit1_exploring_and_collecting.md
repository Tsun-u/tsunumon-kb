# AP Statistics (2026-27) — Unit 1: Exploring One-Variable Data and Collecting Data

> Exam Weight: 20–30% | ~26 Class Periods
> New framework effective fall 2026. Merges former Unit 1 (Exploring One-Variable Data) and Unit 3 (Collecting Data), unified by the statistical investigation process.

## Topics

### 1.1 What Statistical Investigation Looks Like
Every statistical study begins with a genuine question that data can help answer. The four-step cycle — formulate a question, collect data, analyze data, interpret results — frames all of statistics.
- A good investigative question requires data to answer and has a population of interest

### 1.2 Variables
A dataset describes individuals. Each characteristic recorded is a variable.
- **Categorical variables** sort individuals into groups (color, class, yes/no)
- **Quantitative variables** measure numerical quantities for which arithmetic makes sense; can be discrete (countable) or continuous (measured on a scale)

### 1.3 Summarizing One Categorical Variable with Tables
Tables are the starting point for categorical data.
- Frequency tables report the count per category; relative frequency tables report the proportion
- Proportions and percentages describe how each category contributes to the whole

### 1.4 Visualizing One Categorical Variable
Graphs communicate the distribution at a glance.
- Bar charts (frequency and relative frequency), pie charts
- Good graphs make comparisons across categories easy; annotate with context

### 1.5 Visualizing One Quantitative Variable
Several plot types reveal a distribution's shape.
- Histograms, dotplots, stem-and-leaf plots, cumulative frequency graphs

### 1.6 Describing a Quantitative Distribution
A complete description covers four aspects.
- **Shape:** symmetric, skewed left/right, unimodal, bimodal, uniform
- **Center:** where the data tend to pile up
- **Variability (spread):** how spread out the values are
- **Unusual features:** outliers, gaps, clusters — always describe in context

### 1.7 Summary Statistics for One Quantitative Variable
Numbers capture center and spread concisely.
- Mean: $\bar{x} = \frac{\sum x_i}{n}$; median; mode
- Standard deviation: $s_x = \sqrt{\frac{\sum(x_i - \bar{x})^2}{n-1}}$; variance; range; **IQR** $= Q_3 - Q_1$
- **Percentiles** and quartiles; relative position via z-scores: $z = \frac{x - \bar{x}}{s_x}$
- Outlier fences: values below $Q_1 - 1.5 \cdot IQR$ or above $Q_3 + 1.5 \cdot IQR$; or beyond ±2 standard deviations
- Resistant statistics (median, IQR) are not pulled by outliers; non-resistant ones (mean, SD) are

### 1.8 Boxplots as Graphical Summaries
A boxplot represents the five-number summary visually.
- **Five-number summary:** min, $Q_1$, median, $Q_3$, max
- Modified boxplots show outliers as individual points beyond the fences

### 1.9 Comparing Distributions
Side-by-side displays (parallel boxplots, back-to-back stemplots) support group comparisons.
- Compare shape, center, variability, and unusual features for each group
- All comparisons should use comparative language tied to the variable's context

### 1.10 Investigative Questions and Data Collection Planning
Before collecting data, a plan ensures the results can address the question.
- Refine the question; justify the data collection method
- Distinguish population from sample; identify whether the study is an observational study or experiment; consider generalizability and ethics

### 1.11 Random Sampling Methods
Random selection ensures each individual in the population has a known chance of being included.
- **Simple random sample (SRS):** every possible sample of size $n$ is equally likely
- **Stratified random sample:** divide into homogeneous strata; draw an SRS from each
- **Cluster sample:** divide into clusters; randomly select entire clusters
- **Systematic random sample:** select every $k$th unit from a list after a random start
- Random selection supports generalization of results to the larger population

### 1.12 Bias and Limitations in Sampling
No sampling method is immune to problems if poorly executed.
- **Bias sources:** undercoverage, nonresponse, response bias (question wording, interviewer effects), voluntary response, convenience sampling
- A biased method stays biased regardless of sample size

### 1.13 Experimental Design
Experiments manipulate variables and observe outcomes; only experiments with random assignment support causal conclusions.
- **Experimental units:** individuals assigned to treatments
- **Treatments, factors, levels:** the conditions imposed; the variables manipulated; the specific values of those variables
- **Explanatory variable:** what is manipulated; **response variable:** what is measured
- **Principles:** comparison, random assignment, control, replication
- **Designs:** completely randomized, randomized block, matched pairs
- **Confounding variables** make it impossible to separate the effects of the explanatory variable from other factors
- **Placebo effect:** improvement from belief in treatment, not the treatment itself; **blinding** (single and double) controls for this
- Random assignment → cause-and-effect conclusions are supported

## Key Formulas

| Formula | Description |
|---------|-------------|
| $\bar{x} = \frac{\sum x_i}{n}$ | Sample mean |
| $s_x = \sqrt{\frac{\sum(x_i - \bar{x})^2}{n-1}}$ | Sample standard deviation |
| $IQR = Q_3 - Q_1$ | Interquartile range |
| $z = \frac{x - \bar{x}}{s_x}$ | z-score (relative position within a dataset) |

## Common Misconceptions

- **Random sampling ≠ random assignment:** sampling supports generalization; assignment supports causation — they serve different purposes
- **Sample size doesn't fix bias:** a large biased sample is still biased
- **The mean is not resistant:** outliers and skewness pull the mean but not the median
- **Distributions need context:** always describe shape, center, variability, and unusual features in terms of the variable being measured
- **Skew direction:** skewed left means the long tail points left (toward smaller values), not that most data are on the left

## Note on the 2026-27 Restructure

- The **normal distribution** is no longer in this unit — it now appears in Unit 2 as a probability model
- The former standalone "Collecting Data" unit (old Unit 3) is now integrated as Topics 1.10–1.13
