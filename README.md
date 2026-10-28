# 📊 Statistics & Probability for Data Science & Analysis

Welcome to the **Statistics & Probability** repository! This project serves as a comprehensive, hands-on learning hub bridging theoretical statistical concepts with practical Python implementations for data analysis and machine learning.

It includes **37 pages of handwritten theory notes** along with **interactive Jupyter Notebooks** utilizing real-world datasets (such as the Titanic dataset) and Python libraries like NumPy, Pandas, Matplotlib, and Seaborn.

---

## 📁 Repository Structure

```text
Statistics_&_Probability/
│
├── Handwritten Notes for Statistics and Probability/   # 37 Scanned Study Pages
│   ├── CamScanner 10-28-2026 11.15_1.jpg              # Intro & Data Analysis Lifecycle
│   ├── ...                                             # Probability, Sampling, Distributions
│   └── CamScanner 10-28-2026 11.15_37.jpg              # Hypothesis Testing, Chi-Square & Formulas
│
├── Mean_Median_mode.ipynb                              # Measures of Central Tendency
├── Percentile_and_skewness.ipynb                       # Percentiles, Quartiles, Skewness & Boxplots
├── Range_MAD_SD.ipynb                                  # Measures of Spread & Dispersion
└── README.md                                           # Repository Documentation
```

---

## 📓 Jupyter Notebooks Breakdown

### 1. 🎯 [Mean_Median_mode.ipynb](Mean_Median_mode.ipynb)
Focuses on **Measures of Central Tendency** — finding the center point of data distributions:
- **Core Concepts**: Arithmetic Mean ($\bar{x}$), Median (50th percentile), and Mode (most frequent value).
- **Manual vs. Vectorized Calculations**: Array computations using vanilla Python logic vs. optimized `numpy` operations.
- **Dataset Analysis**: Applied directly to the Titanic dataset (`Fare` feature).
- **Missing Value Imputation**: Handling `NaN` entries with mean-based strategy (`fillna`).
- **Visualization**: Frequency distributions plotted with `seaborn.histplot` overlaying vertical lines for Mean, Median, and Mode.

### 2. 📈 [Percentile_and_skewness.ipynb](Percentile_and_skewness.ipynb)
Focuses on **Data Distribution Shape and Relative Standing**:
- **Percentiles & Quartiles**: Calculating arbitrary percentiles ($P_{25}, P_{50}, P_{75}$) using `np.percentile()` and `.describe()`.
- **Outlier Detection**: Visual inspection via Box and Whisker plots (`sns.boxplot`).
- **Skewness Analysis**: Understanding symmetric vs. right-skewed (positive) vs. left-skewed (negative) distributions using `.skew()`.
- **Synthetic Experiments**: Demonstrating how outliers pull the mean away from the median using custom discrete distributions.

### 3. 📏 [Range_MAD_SD.ipynb](Range_MAD_SD.ipynb)
Focuses on **Measures of Dispersion & Spread**:
- **Range**: Difference between maximum and minimum values ($\text{Range} = X_{\max} - X_{\min}$).
- **Mean Absolute Deviation (MAD)**: Average distance of observations from the central mean:
  $$\text{MAD} = \frac{1}{n} \sum_{i=1}^{n} |x_i - \bar{x}|$$
- **Variance ($\sigma^2, s^2$) & Standard Deviation ($\sigma, s$)**: Measuring variability around the mean using NumPy and Pandas functions (`.var()`, `.std()`).
- **Comparative Dispersion**: Side-by-side scatter plots comparing spreads across different cohorts (`sec_a` vs. `sec_b`) relative to a common mean.

---

## 📝 Handwritten Theory Notes

The [`Handwritten Notes for Statistics and Probability/`](Handwritten%20Notes%20for%20Statistics%20and%20Probability/) folder contains complete, high-resolution scanned study sheets covering:

| Topic # | Subject Area | Key Concepts Covered |
|:-------:|:-------------|:---------------------|
| **01 - 04** | **Foundations of Statistics** | Definition of statistics, data analysis lifecycle, descriptive vs. inferential vs. predictive statistics, population vs. sample, parameters vs. statistics, qualitative (nominal/ordinal) vs. quantitative (discrete/continuous) data. |
| **05 - 11** | **Descriptive Statistics** | Measures of central tendency (Mean, Median, Mode), Measures of dispersion (Range, Variance, Standard Deviation, Interquartile Range $IQR = Q_3 - Q_1$). |
| **12 - 17** | **Probability Theory** | Basic probability definitions, sample spaces, Addition Rule ($P(A \cup B)$), Multiplication Rule ($P(A \cap B)$), Independent events, Conditional Probability ($P(A \mid B)$), Complement rule. |
| **18 - 21** | **Sampling & Bias** | Sampling methods (Simple Random, Systematic, Stratified, Cluster, Convenience), sampling bias, and avoiding representative distortion. |
| **22 - 23** | **Hypothesis Testing** | 5-step hypothesis testing framework, Null Hypothesis ($H_0$) vs. Alternative Hypothesis ($H_1$), significance level ($\alpha = 0.05$), test statistics, and p-values. |
| **24 - 25** | **Regression & Chi-Square** | Simple linear regression ($\hat{y} = b_0 + b_1 x$), slope & intercept interpretation, Chi-Square Goodness-of-Fit and Independence test ($\chi^2 = \sum \frac{(O_i - E_i)^2}{E_i}$). |
| **Summary** | **Quick Reference Sheet** | Consolidated formula cheat sheet for standard error ($SE = \frac{s}{\sqrt{n}}$), z-scores, confidence intervals, Pearson correlation, and coefficient of variation ($CV$). |

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.8+ installed along with Jupyter Notebook or JupyterLab.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sharmanageshwor/Statistics-and-probability.git
   cd Statistics-and-probability
   ```

2. **Create a virtual environment (optional but recommended)**:
   ```bash
   python -m venv venv
   # Windows:
   venv\Scripts\activate
   # macOS/Linux:
   source venv/bin/activate
   ```

3. **Install required packages**:
   ```bash
   pip install numpy pandas matplotlib seaborn jupyter
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

---

## 📊 Tech Stack & Tools

- **Language**: Python 3.x
- **Data Manipulation**: [NumPy](https://numpy.org/), [Pandas](https://pandas.pydata.org/)
- **Data Visualization**: [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/)
- **Environment**: [Jupyter Notebook](https://jupyter.org/) / Google Colab

---

## 💡 Notes on Dataset

The notebooks reference `titanic_dataset.csv` (commonly downloaded from Kaggle or Seaborn's built-in datasets). If running locally, you can load it directly via:
```python
import seaborn as sns
dataset = sns.load_dataset('titanic')
```
or place `titanic_dataset.csv` in your working directory.

---

## 🤝 Contributing & Feedback

Contributions, corrections, or additional notebooks (e.g., covering distributions, central limit theorem, or ANOVA) are welcome!
Feel free to open an issue or submit a pull request.


