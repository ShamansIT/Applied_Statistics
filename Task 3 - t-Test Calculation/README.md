# Task 3: t-Test Calculation
![t-Test Calculation](https://www.investopedia.com/thmb/yc7LDieTkD3dl9GYFmvMsNHNfy0=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc()/t-test_final2-d26bbb129cc441c192ccf8e784ae06a4.png)

**by Serhii Spitsyn**

# Description
This project explores effectiveness of two-week exercise program by analyzing changes in resting heart rates of patients before and after the program. Paired t-test is used to determine whether the observed differences in heart rates are statistically significant. The project demonstrates the calculation of the t-statistic manually and then compares it to results from Python’s scipy.stats library.

## Project Stages:
1. Data Preparation: Collect and structure the heart rate data for each patient before and after the exercise program.
2. Manual Calculation of t-Statistic: Compute the t-statistic using the formula for paired samples, based on the mean difference and standard deviation of the differences.
3. t-Test with SciPy: Perform a paired t-test using scipy.stats.ttest_rel to validate the manual calculation.
4. Result Comparison: Compare the t-statistics from the manual calculation and SciPy’s output.
5. Conclusion: Interpret the results to assess if there was a statistically significant effect from the exercise program.

## Purpose of the Project 
The goal of this project is to use statistics to check if a two-week exercise program helped improve health. Focus on whether there’s a real change in resting heart rate, which can show better heart health. This project also helps us practice calculating statistics and using Python for testing ideas.

## Methodology
* **Data Collection:**  
  The dataset includes resting heart rates for 10 patients, recorded before and after the exercise program.

* **Paired t-Test Formula:**  
  For paired data, the t-statistic is calculated using the formula:

  $$
  t = \frac{\text{mean difference}}{\text{standard deviation of the difference} / \sqrt{n}}
  $$

  where **n** is the number of patients, the mean difference represents the average change in heart rate, and the standard deviation of the difference measures variability.

* **Hypothesis Testing with SciPy:**  
  Using `scipy.stats.ttest_rel`, a paired t-test is performed to test the null hypothesis H<sub>0</sub>: there is no significant difference in resting heart rates before and after the program.

## Descriptions
- Data:
The dataset consists of two arrays: before and after, representing resting heart rates for each patient before and after the exercise program, respectively.
- t-Statistic Calculation (Manual):
The t-statistic was manually calculated using the formula above, allowing for a deeper understanding of the process and the components of a paired t-test.
- t-Statistic Calculation (SciPy):
Used the scipy.stats.ttest_rel function to validate our manual calculation, which confirms that the paired t-test can be efficiently conducted with Python.

## Conclusions
As conclusions **can be sure of the accuracy of the calculations and the correctness of the test**.

1.	Precision of Manual Calculations
A very small difference confirms that the manual calculation of the t-statistic was performed correctly and with sufficient accuracy, using formulas for the mean and standard deviation of the differences.
2.	Reliability of the SciPy library
Since the scipy.stats result is virtually identical to our manual calculation, this confirms the reliability and accuracy of the SciPy library for statistical tests in Python.
3.	Machine error
The difference between calculations can be explained as machine error, which occurs due to the limited precision of floating-point numbers in computing systems. This error is normal and does not affect the results of the analysis.

### Final Thoughts
This project provides a practical example of using the paired t-test for health data analysis, helping to reinforce the process of hypothesis testing in Python. By performing calculations both manually and with SciPy, gained a clearer understanding of the t-test's components and its application to real-world data.

## Next steps witch was done
The following actions were completed in the project:
1.	Collection and structuring of data for analysis.
2.	Step-by-step calculation of the t-statistic manually.
3.	Application of scipy.stats.ttest_rel for automated testing.
4.	Comparison of manual and automated results.
5.	Interpretation of the significance of the findings.

Potential future steps could involve applying similar statistical tests to larger datasets or exploring other health metrics to evaluate program effectiveness. This analysis can also serve as foundation for future work in health data analytics.

## Project structure
The project consists of the following files and directories:
- 'task3_t-Test_Calculation.ipynb' is the main Jupyter Notebook, where calculations and explanations are performed.
- 'README.md' — project description and instructions.

## Requirements
To complete the project, you must have:
- Python 3.8+
- Jupyter Notebook
- SciPy
- NumPy

### Contribution to the project
Contributions are welcome! You can help improve the project by opening an issue or creating a pull request.

## Reference
- [SciPy Documentation - t-Test](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_rel.html)
- [NumPy Introduction](https://www.w3schools.com/python/numpy/numpy_intro.asp)
- [An introduction to t-test theory for surveys](https://www.qualtrics.com/en-gb/experience-management/research/t-test/)
- [The Paired t-Test and Exercise Programs](https://www.ncbi.nlm.nih.gov/)
- [Real Statistics Using Excel – Paired t-Test](https://statisticsbyjim.com/hypothesis-testing/t-tests-excel/)
- [Real Statistics – Paired t-Test](https://statisticsbyjim.com/hypothesis-testing/t-tests-excel/)

## Contact Information
- <serhii.spitsyn.ie@gmail.com>
- [GitHub](https://github.com/ShamansIT)