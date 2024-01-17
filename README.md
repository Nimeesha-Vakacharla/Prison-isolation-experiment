# Prison-isolation-experiment
## QUESTION
Subjects from Central Prison in Raleigh, NC, volunteered for an experiment involving an "isolation" experience. The goal of the experiment was to find a treatment that reduces subjects' psychopathic deviant T scores. This score measures a person's need for control or their rebellion against control, and it is part of a commonly used mental health test called the Minnesota Multiphasic Personality Inventory (MMPI) test. 

The experiment had three treatment groups:
(1) Four hours of sensory restriction plus a 15 minute "therapeutic" tape advising that professional help is available.
(2) Four hours of sensory restriction plus a 15 minute "emotionally neutral" tape on training hunting dogs.
(3) Four hours of sensory restriction but no taped message.

Forty-two subjects were randomly assigned to these treatment groups, and an MMPI test was administered before and after the treatment.
## Steps of Approch 
### Statistical test
1. In the context of conducting a statistical test, the test statistic serves as a numerical representation of how closely the distribution of observed data aligns with the expected distribution under the null hypothesis. Subsequently, the calculated test statistic is utilized in determining the p-value, or probability value, which, in turn, is instrumental in deciding whether to accept or reject the null hypothesis.
2. The presence of a statistically significant relationship between predictor and outcome variables is implied when the test statistic surpasses the value derived from the null hypothesis. This comparison serves as an indicator of the strength of the association between the variables.
3. Conversely, if the computed test statistic falls short of the extremeness observed in the null hypothesis, it suggests the absence of a statistically significant relationship between the predictor and outcome variables. This discrepancy emphasizes the importance of interpreting the test statistic in gauging the significance of the observed relationship.
### When to perform a statistical test?
1. Statistical analyses are employed when researchers pose specific research questions involving group comparisons, relationship assessments, or hypothesis testing.
2. The selection of a statistical test is contingent upon the nature of the data. For instance, ANOVA is suitable for scenarios with three or more groups, while t-tests are apt for comparing means between two groups.
3. A statistical test's validity hinges on the adequacy of the sample size, ensuring it is large enough to approximate the true distribution of the population under investigation.
4. The study's design, whether experimental or observational, dictates the choice of an appropriate statistical test. Experimental designs commonly utilize ANOVA or t-tests, whereas observational studies may employ correlation or regression. To determine the suitable statistical test:
   - It is imperative to confirm whether the data satisfies specific assumptions.
   - Consideration must be given to the types of variables under analysis (categorical, continuous, dependent, independent).
### Statistical Assumptions
Statistical tests rely on certain fundamental assumptions concerning the data under examination. These assumptions include:

```Normality```: Numerous statistical tests presuppose that the data conforms to a normal distribution. Deviations from this assumption can potentially undermine the dependability of the results.

```Independence```: The assumption of independence stipulates that observations within the dataset should be unrelated to each other. For instance, in a t-test, values within one group should not exhibit correlations with values in another group.

```Homogeneity of Variance```: Homogeneity assumes that the variances among the groups being compared are approximately equal. Violations of this assumption have the potential to impact the accuracy and reliability of the statistical test.
### Types of test statistics

Below is a summary of the most common test statistics, their hypotheses, and the types of statistical tests that use them.
| Test Statistic |             Null and Alternative Hypotheses                | Statistical Tests |
| :------------  |:----------------------------------------------------------:|------------------:|
|    t-value     | Null: The means of two groups are equal                    |      T-test       |
|                | Alternative: The means of two groups are not equal         |                   |
|    z-value     | Null: The means of two groups are equal                    |      Z-test       |
|                | Alternative: The means of two groups are not equal         |                   |
|    F-value     | Null: The means of all groups are equal                    |      ANOVA        |
|                | Alternative: The means of atleast two groups are not equal |                   |

### ANOVA (Analysis of Variance)

The Analysis of Variance, abbreviated as ANOVA, is a statistical procedure employed to assess the presence of significant differences among the means of three or more independent sets of continuous data. Introduced by Ronald Fisher in 1918, this test is frequently applied in experimental designs featuring multiple independent groups.
One way and Two way ANOVA
1. One-way or two-way refers to the number of independent variables in the ANOVA test.
2. In one-way ANOVA, we assess the impact of a single factor on a response variable to determine if there are statistically significant differences among the means of three or more independent groups.
3. Two-way ANOVA (Analysis of Variance) is a statistical technique that extends the one-way ANOVA to assess the impact of two independent variables simultaneously on a dependent variable

### Steps of Computation
1. This study investigates the impact of sensory restriction on psychopathic deviant T scores among subjects from Central Prison in Raleigh, NC. The experiment aimed to identify a treatment that could effectively reduce individuals' tendencies toward the need for control or rebellion against control, as measured by the Minnesota Multiphasic Personality Inventory (MMPI) test.
2. Exploratory Data Analysis (EDA) techniques were applied to understand the initial trends and variations in the data by generating box plots, while a One-Way Analysis of Variance (ANOVA) was employed to assess the significance of differences among the three treatment groups
3. Generate the Null and Alternative Hypotheses for the provided data set. Descriptive statistics such as means, variances, standard deviations, and sum of squares will be computed to obtain F-test statistics.
4. We Reject or accept the Null Hypothesis based on the F statistics.
5. To reject the null hypothesis, the Bonferroni Correction Method will be employed for pairwise comparisons, to identify which treatment groups differ from each other.
6. The findings from this study contribute valuable insights into the potential efficacy of sensory restriction as a therapeutic approach for reducing psychopathic deviant T scores, with implications for the development of interventions within correctional settings.

### Conclusion

From the ANOVA analysis, the p-value linked to the "treatments" factor stands at 0.046069. This value falls below the conventional significance threshold of 0.05, providing substantial evidence to reject the null hypothesis asserting equality of means among the treatment groups.

Within the post hoc comparison results, the p-values corresponding to specific pairwise comparisons between treatments are evident. Notably, the "diff_of_trt3 - diff_of_trt1" comparison yields a p-value, falling below the modified significance level of 0.017. This indicates a statistically significant difference between the means of "diff_of_trt3" and "diff_of_trt1."

Conducting Bartleet, Levene, and Shapiro-Wilk tests, the derived p-value from our ANOVA analysis is deemed significant. Consequently, we fail to reject the null hypothesis, indicating that the collected data adheres to a normal distribution and fulfills the assumption of homogeneity of variances.

In conclusion, based on both the overall ANOVA test and the post hoc comparisons, we reject the null hypothesis for the "treatments" factor overall, indicating that there are significant differences among at least some of the treatment groups.
