# Task 1: Permutations and Combinations
![Lady Tasting Tea](https://e10v.me/tea-tasting-rdd/lady-tasting-tea-small.png)

**by Serhii Spitsyn**

# Description

## Purpose of the Project 

This project performs probability analysis using combinatorics methods to solve a modified experiment reminiscent of "Lady Tasting Tea." In this scenario, there are 12 cups of tea: 6 of them with milk added first and 6 with tea added first. The task is to calculate the probability that a person, guessing randomly, can correctly identify all 6 cups of milk added first. Additionally, we analyze the probability that the person can make one or two mistakes and still be considered successful.

## Methodology

We use combinatorics formulas and Python's `math.comb()` function to calculate the number of possible combinations when choosing 6 cups out of 12. Below are the key steps and formulas used in the analysis:

### 1. Total number of combinations

The total number of ways to choose 6 cups from 12 is given by the binomial coefficient formula:

$$
C_{12}^{6} = \frac{12!}{6! \times 6!}
$$

Using this formula, we can calculate the total number of possible combinations for selecting 6 cups out of 12.

### 2. Probability of guessing all 6 cups correctly

Since there is only **one way** to guess all 6 cups correctly (the person selects exactly the correct 6 cups), the probability of this event is:

$$
P(\text{всі правильні}) = \frac{1}{C_{12}^{6}} = \frac{1}{924}
$$

This is an extremely small probability, indicating that guessing all cups correctly by chance is highly unlikely.

### 3. Probability of guessing exactly 5 cups correctly

To calculate the probability of guessing exactly 5 correct cups, we use the following reasoning:

- The number of ways to choose exactly 5 correct cups from the 6 correct ones is:

$$
C_6^5 = \frac{6!}{5! \times 1!} = 6
$$

- The number of ways to choose 1 incorrect cup from the remaining 6 incorrect ones is:

$$
C_6^1 = 6
$$

Thus, the total number of favorable outcomes for guessing exactly 5 cups correctly is:

$$
C_6^5 \times C_6^1 = 6 \times 6 = 36
$$

The probability of guessing exactly 5 cups correctly is:

$$
P(\text{5 правильних}) = \frac{36}{C_{12}^{6}} = \frac{36}{924} = 0.03896
$$

### 4. Probability of making no more than one mistake

To calculate the probability of making no more than one mistake (either guessing all 6 correctly or exactly 5 correctly), we sum the favorable cases for both:

$$
\text{Сприятливі комбінації для не більше однієї помилки} = C_6^6 \times C_6^0 + C_6^5 \times C_6^1
$$

This gives us:

$$
1 + 36 = 37
$$

Thus, the probability of making no more than one mistake is:

$$
P(\text{не більше однієї помилки}) = \frac{37}{C_{12}^{6}} = \frac{37}{924} = 0.0400
$$

### 5. Probability of guessing exactly 4 cups correctly

To calculate the probability of guessing exactly 4 cups correctly, we again use combinations:

- The number of ways to choose 4 correct cups from the 6 correct ones is:

$$
C_6^4 = \frac{6!}{4! \times 2!} = 15
$$

- The number of ways to choose 2 incorrect cups from the remaining 6 incorrect ones is:

$$
C_6^2 = \frac{6!}{2! \times 4!} = 15
$$

Thus, the total number of favorable outcomes for guessing exactly 4 cups correctly is:

$$
C_6^4 \times C_6^2 = 15 \times 15 = 225
$$

The probability of guessing exactly 4 cups correctly is:

$$
P(\text{4 правильних}) = \frac{225}{C_{12}^{6}} = \frac{225}{924} = 0.2435
$$

### 6. Probability of making no more than two mistakes

To calculate the probability of making no more than two mistakes (i.e., guessing all 6, 5, or 4 correctly), we sum the favorable cases for these events:

$$
\text{Сприятливі комбінації для не більше двох помилок} = C_6^6 \times C_6^0 + C_6^5 \times C_6^1 + C_6^4 \times C_6^2
$$

This gives us:

$$
1 + 36 + 225 = 262
$$

Thus, the probability of making no more than two mistakes is:

$$
P(\text{не більше двох помилок}) = \frac{262}{C_{12}^{6}} = \frac{262}{924} = 0.2831
$$

## Conclusions

### 1. Probability of guessing all 6 cups correctly
The probability of guessing all 6 cups correctly is extremely low, at:

$$
P(\text{всі правильні}) = \frac{1}{924} \approx 0.0011
$$

This shows that it is highly unlikely for a person to guess all 6 cups correctly by chance.

### 2. Probability of making no more than one mistake
The probability of making no more than one mistake is still quite low, at:

$$
P(\text{не більше однієї помилки}) = \frac{37}{924} \approx 0.0400
$$

This indicates that allowing for one mistake still results in a small probability of success by guessing.

### 3. Probability of making no more than two mistakes
The probability of making no more than two mistakes is significantly higher, at:

$$
P(\text{не більше двох помилок}) = \frac{262}{924} \approx 0.2831
$$

This suggests that if we allow for two mistakes, the likelihood of guessing successfully increases to about 28%, which is too high to be considered a valid test of a person's ability to correctly identify the order of tea and milk.

### Final Thoughts
- The probability of guessing all 6 cups correctly is minuscule, indicating the near impossibility of doing so by chance.
- Allowing for one mistake still keeps the probability of random success low (around 4%).
- Allowing for two mistakes, however, significantly increases the chance of success to 28%, which is too high to confidently claim that the person possesses any special ability based solely on this test.

Thus, it is reasonable to accept a claim of special ability if the person makes no more than **one mistake**. Allowing more errors compromises the validity of the test, as the probability of random success becomes unacceptably high.

## Next steps
The study can be expanded to examine cases with larger cup sets or other selection scenarios where the number of items may vary.

## Project structure
The project consists of the following files and directories:
- 'tasks.ipynb' is the main Jupyter Notebook, where calculations and explanations are performed.
- 'README.md' — project description and instructions.

## Requirements
To complete the project, you must have:
- Python 3.8+
- Jupyter Notebook
- 'math'Lib (built into Python)

### Contribution to the project
Contributions are welcome! You can help improve the project by opening an issue or creating a pull request.

## Reference
- [Lady tasting tea experement](https://lisds.github.io/textbook/wild-pandas/fishers_tea.html)
- [Python math — Mathematical functions 'comb'](https://docs.python.org/3/library/math.html#math.comb)
- [The lady tasting tea experiment](https://brainder.org/2015/08/23/the-lady-tasting-tea-and-fishers-exact-test/)
- [Readme Driven Development for an A/B testing analysis package](https://e10v.me/tea-tasting-rdd/)

## Contact Information
- <serhii.spitsyn.ie@gmail.com>
- [GitHub](https://github.com/ShamansIT)