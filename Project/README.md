# Plant Growth Dataset Analysis
![Plant Growth Analysis](https://www.ie.edu/insights/wp-content/uploads/2023/02/Beinish-Feature-v2.gif)

**by Serhii Spitsyn**

# Description
This project involves analyzing the PlantGrowth dataset, which includes data on plant weights across three groups: a control group (ctrl) and two treatment groups (trt1 and trt2). The analysis employs statistical techniques such as t-tests and ANOVA to determine if there are significant differences between these groups.

## Project Stages:
1.	Data Loading: The dataset is loaded and cleaned for analysis.
2.	Exploratory Data Analysis: Descriptive statistics and visualizations provide an overview of the data.
3.	T-Test: A t-test is conducted to compare the mean weights between two treatment groups.
4.	ANOVA: ANOVA is performed to evaluate differences among all three groups.
5.	Documentation: Findings are summarized, and a report is generated.
6.	Conclusion: Final insights and observations are presented.

## Purpose of the Project 
The primary goal of this project is to:
- Identify significant differences in plant weights between groups.
- Demonstrate the use of statistical techniques such as t-tests and ANOVA in real-world scenarios.
- Provide insights into the effects of treatments on plant growth.

## Methodology
- T-Test: Used to compare means between trt1 and trt2 groups, ensuring assumptions of normality and equal variances are met.
- ANOVA: Applied to analyze differences among all three groups while controlling for multiple comparisons.

## Descriptions
- Dataset:
    - weight: Numeric variable representing the dried weight of plants.
    - group: Categorical variable representing treatment groups (ctrl, trt1, trt2).
- T-Test:
    - Compares trt1 and trt2 to assess statistical significance.
- ANOVA:
    - Evaluates differences across ctrl, trt1, and trt2 groups.

## Conclusions
- Key Findings:
    - Significant differences were identified between the treatment groups.
    - ANOVA highlighted differences among all three groups.
- Practical Implications:
    - Results provide insights into the effectiveness of treatments.

### Final Thoughts
This analysis demonstrates the value of statistical methods in experimental research. By leveraging Python libraries and robust statistical techniques, meaningful conclusions about the dataset were derived.

## Project structure
project/
  |-- PlantGrowth.csv         # Contains the PlantGrowth dataset
  |-- project.ipynb           # Jupyter Notebook with analysis
  |-- Readme.md               # Documentation

## Requirements
- Python 3.7 or later
- Required Libraries:
    - pandas
    - scipy
    - matplotlib
    - seaborn

### Contribution to the project
Contributions are welcome! Please ensure your code adheres to the existing style and structure. Submit pull requests with clear descriptions of changes.

## Reference
- [An Introduction to Statistical Modelling](https://www.scribd.com/document/420199566/Introduction-to-Statistical-Modelling-pdf)
- [Numpy Testing guidelines](https://numpy.org/devdocs/reference/testing.html)
- [ANOVA Test: An In-Depth Guide with Examples](https://www.datacamp.com/tutorial/anova-test)
- [ANOVA, Single + Multiple, Factors, Lending Club data](https://s3.amazonaws.com/assets.datacamp.com/production/course_6572/slides/chapter2.pdf)
- [Getting Started With Testing in Python](https://realpython.com/python-testing/)
- [Statistical Analysis in Biology](https://www.studysmarter.co.uk/explanations/biology/biology-experiments/statistical-analysis-in-biology)
- [Matplotlib 3.10.0 documentation](https://matplotlib.org/stable/index.html)
- [Seaborn: statistical data visualization](https://seaborn.pydata.org/)

## Contact Information
- <serhii.spitsyn.ie@gmail.com>
- [GitHub](https://github.com/ShamansIT)