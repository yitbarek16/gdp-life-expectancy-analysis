# 📊 GDP vs Life Expectancy — 2013 (World Bank)

Overview
--------

This project examines the relationship between a country's total GDP and average life expectancy using World Bank data for the year 2013. The analysis explores correlations, demonstrates limitations of aggregate indicators, and provides a reproducible notebook to reproduce the results and visuals.

Why this project matters
------------------------

- 🔎 **Question:** Do richer countries (by total GDP) have longer life expectancy?
- ⚠️ **Caveat:** Total GDP is not normalized by population — consider `GDP per capita` for fairer comparisons.

Datasets
--------

- `datasets/WB GDP 2013.csv` — World Bank indicator `NY.GDP.MKTP.CD` (GDP, current US$)
- `datasets/WB LE 2013.csv` — World Bank indicator `SP.DYN.LE00.IN` (Life expectancy at birth)

Quick Objectives
----------------

- ✨ Clean and prepare the two datasets
- 🔁 Convert/format GDP into readable units (millions) and convert currency where applicable
- 🔗 Merge by country and handle missing/aggregate rows
- 📈 Measure correlation (Spearman rank) and visualize using a log-scaled scatter plot

Methodology (brief)
-------------------

- Remove aggregated country groups and rows with missing values
- Convert GDP to a readable unit (millions) and, if shown in USD, optionally convert to GBP in the notebook
- Round life expectancy values for clarity
- Perform an inner join on country names and compute Spearman rank correlation
- Create a scatter plot (GDP on log scale) and annotate notable outliers

Key Findings
------------

- 📊 A moderate positive correlation (~0.50) is observed between total GDP and life expectancy in 2013.
- ⚖️ Correlation is statistically significant but not strong — many exceptions exist.
- 🌍 Total GDP alone is a weak proxy for population well-being; GDP per capita and health spending are more informative.


Tech stack
----------

- Python 3.x
- pandas, scipy, matplotlib
- Jupyter Notebook

## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and share this project with proper attribution.

## 🌟 About Me

Hi there! I'm **Yitbarek Tesfaye**. I’m a Data Professional.
Let's stay in touch! Feel free to connect with me on Linkedin:

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yitbarektesfaye)
