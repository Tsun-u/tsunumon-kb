# Unit 3: Collecting Data
> Exam Weight: 12–15% | ~9–10 Class Periods
> ⚠️ **Legacy 2020 framework unit** (last exam May 2026). Content now in **new Unit 1** (Topics 1.10–1.13). See [index_ap_stats.md](https://tsun-u.github.io/tsunumon-kb/math/index_ap_stats.md).

## Topics

### 3.1 Studies and What They Can Show
The type of study determines what conclusions are possible.
- An **observational study** watches and records variables without deliberately intervening
- An **experiment** applies a treatment and observes the response — this is the only design that can establish cause-and-effect
- Observational studies can reveal associations but not causal links

### 3.2 Populations, Samples, and Censuses
Every study targets a group; rarely is that group fully observed.
- **Population:** the full group of individuals about which we want information
- **Sample:** the subset of the population from which data are actually collected
- **Census:** an attempt to collect data from every individual in the population
- Good study design minimizes bias and reduces unnecessary variability

### 3.3 Sampling Methods
How we select a sample affects whether results can be generalized to the population.
- **Simple Random Sample (SRS):** every possible sample of size $n$ has an equal chance of selection
- **Stratified random sample:** divide the population into homogeneous strata; draw an SRS from each stratum
- **Cluster sample:** divide the population into groups (often geographic); randomly select entire clusters and survey everyone in them
- **Systematic sample:** select every $k$th individual from a list after a random starting point
- **Convenience sample:** selecting whoever is easiest to reach — not a probability method and prone to bias
- Probability-based sampling methods support generalizing results to the broader population

### 3.4 Bias in Sampling
Even a carefully designed study can produce biased results.
- **Undercoverage:** some segments of the population are not represented in the sampling frame
- **Nonresponse bias:** selected individuals do not respond or cannot be reached
- **Voluntary response bias:** people self-select into the sample, over-representing those with strong opinions
- **Response bias:** question wording, interviewer presence, or social pressure distort how people answer
- **Selection bias:** the sampling method systematically favors certain outcomes
- A larger sample does not fix a flawed sampling method — bias is about the method, not the sample size

### 3.5 Experiments: Key Components
An experiment has identifiable structural elements.
- **Explanatory variable (factor):** the variable deliberately manipulated by the researcher
- **Response variable:** the outcome measured to assess the treatment's effect
- **Treatments:** the specific conditions imposed on experimental units
- **Experimental units (subjects):** the individuals or objects assigned to treatments
- **Confounding variable:** a variable that is associated with both the explanatory and response variables, making it impossible to separate their effects
- **Lurking variable:** an unmeasured variable that may influence the observed relationship

### 3.6 Principles of Experimental Design
Three core principles protect against bias and allow valid conclusions.
- **Control:** hold extraneous variables constant across treatment groups to reduce confounding
- **Randomization:** assign treatments randomly so that groups are comparable at the start
- **Replication:** use enough experimental units so that the results are not dominated by chance variation

Common experimental designs:
- **Completely Randomized Design (CRD):** all units are randomly assigned to treatment groups
- **Randomized Block Design:** group units into blocks of similar individuals, then randomize within each block
- **Matched Pairs Design:** a special case of blocking — compare two treatments on paired subjects or on the same subject under both conditions
- **Control group:** a group receiving no treatment or a placebo, serving as the baseline for comparison
- **Blinding:** single-blind if subjects don't know which treatment they received; double-blind if neither subjects nor evaluators know
- **Placebo effect:** subjects sometimes respond simply because they believe they are being treated

### 3.7 Scope of Conclusions
Study design determines what can be concluded.
- **Random sampling** → results can be generalized to the population
- **Random assignment** → causal conclusions can be drawn

| | Random Assignment | No Random Assignment |
|---|---|---|
| **Random Sample** | Cause-and-effect + generalizable to population | Association + generalizable to population |
| **No Random Sample** | Cause-and-effect (for the group studied) | Association (for the group studied) |

- **Statistical significance:** an observed result large enough that chance alone is an unlikely explanation
- When statistically significant results come from an experiment with random assignment, a causal conclusion is supported

## Common Misconceptions
- Confusing **random sampling** (supports generalization) with **random assignment** (supports causation) — this is the most common conceptual error in study design
- Believing a large sample eliminates bias — a biased sampling method remains biased regardless of how many people are sampled
- Confusing **stratified** and **cluster** sampling — stratified takes samples within each group; cluster surveys entire selected groups
- Thinking observational studies can prove causation — without random assignment, confounding remains a threat
- Assuming that statistical controls in analysis can fully remove confounding from an observational study — they cannot
