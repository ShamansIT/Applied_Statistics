# Task 4:ANOVA Type II Error Analysis
![ANOVA](https://www.investopedia.com/thmb/DtBF1qar0c5euf4cbG5VqHQ4dZg=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/Analysis-of-Variance-046c809d7efa49d98ea53c4b232a86e8.jpg)

**by Serhii Spitsyn**

# Description
This project explores the probability of committing a Type II error in one-way ANOVA tests under specific conditions. Type II error occurs when the null hypothesis is not rejected despite actual differences existing between the groups. The project uses simulations to evaluate this probability and visualize the results.

## Project Stages:

## Purpose of the Project 
The goal of this project is to:
1. Understand the behavior of Type II errors in one-way ANOVA tests.
2. Explore the effect of sample size, variability, and group means on error rates.
3. Provide insights into statistical hypothesis testing through practical implementation.

## Methodology
1. **Simulations**:
   - Used `numpy.random.normal` to generate data with specific mean and standard deviation for three groups.
   - Conducted one-way ANOVA using `scipy.stats.f_oneway`.
   - Evaluated p-values to detect Type II errors.
2. **Analysis**:
   - Counted the number of tests where Type II errors occurred.
   - Calculated the error rate as a proportion of the total number of tests.

## Descriptions
### Data Parameters:
- **Sample Size**: 100 per group.
- **Standard Deviation**: 0.1.
- **Means**: 4.9, 5.0, and 5.1 for the three groups.

### Simulation Details:
- **Iterations**: 10,000 ANOVA tests performed.
- **Error Criterion**: p-value > 0.05 (indicating failure to reject the null hypothesis).

### Output:
- **Type II Error Count**: Total number of Type II errors observed.
- **Error Rate**: Ratio of Type II errors to total simulations.

## Conclusions
1. The probability of committing a Type II error was calculated and presented as a rate.
2. Results highlighted how slight differences in means can result in statistical challenges when sample size and variability are limited.
3. Visualization using a pie chart provided a clear representation of the findings.

### Final Thoughts
This project demonstrates the importance of understanding Type II errors in hypothesis testing. While Type I errors are often emphasized, Type II errors play a critical role in determining the efficacy of statistical tests and study designs. 

## Project structure
The project consists of the following files and directories:
- 'task4_ANOVA.ipynb' is the main Jupyter Notebook, where calculations and explanations are performed.
- 'README.md' — project description and instructions.

## Requirements
To complete the project, you must have:
- Python 3.8+
- Jupyter Notebook

### Contribution to the project
Contributions are welcome! You can help improve the project by opening an issue or creating a pull request.

## Reference
- [ANOVA for unbalanced data: Use Type II instead of Type III sums of squares](http://www.stat.yale.edu/~jtc5/312_612/readings/unbalanced_two-way_anova_and_interactions/unbalanced-anova-use-type-II-SS_Stat-Comput_03.pdf)
- [Anova - Type I/II/III SS explained](https://www.r-bloggers.com/2011/03/anova-%E2%80%93-type-iiiiii-ss-explained/)
- [Analysis of variance](https://en.wikipedia.org/wiki/Analysis_of_variance)
- [ANOVA Test: Definition, Types, Examples, SPSS](https://www.statisticshowto.com/probability-and-statistics/hypothesis-testing/anova/)


## Contact Information
- <serhii.spitsyn.ie@gmail.com>
- [GitHub](https://github.com/ShamansIT)