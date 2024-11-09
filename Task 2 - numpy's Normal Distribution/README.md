# Task 2: Numpy's Normal Distribution
![Normal Distribution](https://cdn.analyticsvidhya.com/wp-content/uploads/2021/05/51240maxresdefault.jpg)

**by Serhii Spitsyn**

# Description
This task checks whether the numpy.random.normal() function correctly generates values ​​from a normal distribution.

## Project Stages:
- Generate a sample of 100,000 values with a mean of 10.0 and a standard deviation of 3.0.
- Provide Shapiro-Wilk test using scipy.stats.shapiro() to check the normality of the sample distribution.
- Constructing histogram of the obtained values and superimposing on it the corresponding probability density function of the normal distribution.

## Purpose of the Project 
The purpose of this project is to evaluate whether numpy.random.normal() properly generates values that follow a normal distribution with given parameters. Specifically testing large sample of values generated with a mean (μ) of 10.0 and a standard deviation (σ) of 3.0. Aim to verify this distribution by using statistical tests and visualizations, checking if the generated sample aligns with the characteristics of a theoretical normal distribution.

## Methodology
- **Generate Sample Data**:
Using numpy.random.normal(), generate a sample of 100,000 values with the specified mean (μ = 10.0) and standard deviation (σ = 3.0). This large sample size allows us to approximate the underlying distribution more accurately.

- **Statistical Test for Normality**:
To validate whether our sample truly resembles a normal distribution, apply the Shapiro-Wilk Test, a commonly used method to assess normality. The test examines the null hypothesis H<sub>0</sub>: the data originates from a normal distribution. A p-value greater than 0.05 suggests that fail to reject H<sub>0</sub>, indicating that the data likely follows a normal distribution.

- **Visualization**:
Plot histogram of the sample data to show its empirical distribution. Additionally, add overlay the probability density function of a normal distribution with mean (μ) = 10.0 and standard deviation (σ) = 3.0. This allows us to visually compare the sample data with the theoretical distribution.

## Descriptions
**Normal Distribution**: A continuous probability distribution described by its mean (μ) and standard deviation (σ). In a normal distribution, data tends to cluster around the mean, with symmetrical tails on both sides. Approximately 68% of data falls within one standard deviation from the mean, 95% within two, and 99.7% within three.

**Shapiro-Wilk Test**: A statistical test for normality. The test statistic measures how closely the sample aligns with a normal distribution. The null hypothesis H<sub>0</sub> assumes normality, which can either reject or fail to reject based on the p-value:

p > 0.05: Do not reject H<sub>0</sub>
​
 ; the data is likely normally distributed.
p ≤ 0.05: Reject H<sub>0</sub>; the data likely deviates from normality.

**Histogram and Overlay**: Histogram provides a visual representation of the frequency distribution of our sample data. Overlaying of the theoretical normal distribution allows for a direct comparison, helping us verify that the sample behaves as expected for a normal distribution.

## Conclusions
Based on the results of the Shapiro-Wilk test and the graphical comparison, the following conclusions can be drawn:

- **Normality Validation**:
If the p-value from the Shapiro-Wilk test is greater than 0.05, have no evidence to reject the null hypothesis, suggesting that the sample data is indeed normally distributed. This indicates that numpy.random.normal() generates values that adhere to a normal distribution with the specified parameters.

- **Graphical Verification**:
The histogram of the sample data aligns closely with the overlaid of the normal distribution, visually confirming that the generated data follows the intended distribution with mean 10.0 and standard deviation 3.0.

### Final Thoughts
This project demonstrates that numpy.random.normal() can reliably produce sample that aligns with theoretical expectations for normal distribution. Statistical and graphical methods are complementary: the Shapiro-Wilk test provides quantitative validation, while the histogram and overlay offer visual verification.

## Interesting Examples of the Normal Distribution in Everyday Life
**only for get more attention to Normal Distribution**

The normal distribution often appears in nature and everyday life, though people are rarely notice it. Here are some interesting examples that affect everyone’s life:

- **Human Height and Weight**:
Most people’s height and weight follow a normal distribution, where the mean value represents the average height/weight in a population. This helps doctors and dietitians assess health based on average measurements.

- **Grades in Educational Institutions**:
Exam or test scores in large student groups are often normally distributed: most students achieve average scores, while very high and very low scores are less common. This helps determine the "norm" for academic performance and understand how other students perform.

- **Manufacturing Errors**:
In manufacturing processes, such as making parts for machines or electronics, deviations in part dimensions often follow a normal distribution. This allows manufacturers to predict how many products will meet quality standards.

- **Task Completion Time**:
If a large group of people is given similar tasks, the time taken to complete them generally follows a normal distribution: most will finish in approximately the average time, with only a few finishing significantly faster or slower.

- **Measurement Errors**:
In science and engineering, measurements often have errors, which typically follow a normal distribution. This allows researchers to account for probable deviations in results and improve the accuracy of studies.

**These examples show how the normal distribution impacts many aspects of our lives: from health and education to manufacturing and even economics.**

## Next steps witch was done
- **Explore Other Distributions**:
Generate and evaluate samples from other distributions (e.g., exponential, uniform) to compare their characteristics and apply similar validation methods.

- **Advanced Normality Tests**:
Incorporate additional tests for normality, such as the Kolmogorov-Smirnov or Anderson-Darling tests, to further validate normality in diverse scenarios.

- **Parameter Tuning and Robustness**:
Analyze how changes in sample size, mean, or standard deviation affect the accuracy of the generated normal distribution, assessing the robustness of numpy.random.normal() across different conditions.

- **Practical Applications**:
Apply the generated normal data to real-world simulations or scenarios that require normally distributed data, such as Monte Carlo simulations or financial modeling.

## Project structure
The project consists of the following files and directories:
- 'task2_numpy's_Normal_Distribution.ipynb' is the main Jupyter Notebook, where calculations and explanations are performed.
- 'README.md' — project description and instructions.


## Requirements
To complete the project, you must have:
- Python 3.8+
- Jupyter Notebook
- NumPy
- SciPy
- Matplotlib


### Contribution to the project
Contributions are welcome! You can help improve the project by opening an issue or creating a pull request.

## Reference
- [Normal Distribution : An Ultimate Guide](https://www.analyticsvidhya.com/blog/2021/05/normal-distribution-an-ultimate-guide/)
- [numpy.random.normal](https://numpy.org/doc/2.0/reference/random/generated/numpy.random.normal.html)
- [stats.shapiro](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.shapiro.html)
- [matplotlib.pyplot](https://matplotlib.org/stable/api/pyplot_summary.html)
- [Normal Distribution](https://docs.scipy.org/doc/scipy/tutorial/stats/continuous_norm.html)
- [Wikipedia - Shapiro-Wilk Test](https://en.wikipedia.org/wiki/Shapiro%E2%80%93Wilk_test)
- [The Shapiro-Wilk and related tests for normality](https://math.mit.edu/~rmd/465/shapiro.pdf)
- [Python Data Science Handbook - Probability Distributions](https://medium.com/@patil.manojkumar/probability-distributions-in-python-a-practical-guide-for-beginners-3164f198a398)


## Contact Information
- <serhii.spitsyn.ie@gmail.com>
- [GitHub](https://github.com/ShamansIT)