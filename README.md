# Is a College Degree Worth It? Education, Race, Earnings, and AI

## Project Overview

As a first-generation African American college student, I spent quite a bit of time deciding whether college was worth the cost for me and my family. For this project, I wanted to explore whether having a bachelor's degree or higher is associated with higher annual earnings among Black and White adults ages 22–34 across the United States. I also wanted to look at how AI is being used across occupations and what that could mean for the value of a college degree.

## Data Sources

I used three datasets:

- **2024 American Community Survey (ACS):** Individual-level information on education, earnings, race, age, and employment from the U.S. Census Bureau.
- **Anthropic Economic Index:** Information on AI exposure across occupations.
- **Federal Reserve Bank of New York:** Information on wages, unemployment, and underemployment among recent college graduates.

## Methods

I used Python, pandas, matplotlib, and statsmodels to clean the data, create visualizations, and run a multivariate OLS regression. My main explanatory variable was having a bachelor's degree or higher, and my dependent variable was annual earnings.

I controlled for age and sex and included an interaction between race and education to see whether the relationship differed between Black and White adults. I also used HC3 robust standard errors because my diagnostic tests showed evidence of heteroskedasticity.

## Key Findings

My regression included 57,507 observations. Having a bachelor's degree or higher was associated with earning about $34,288 more annually for White adults and $32,304 more for Black adults, holding age and sex constant.

Although the estimated college earnings advantage was smaller for Black adults, the difference between racial groups wasn't statistically significant at the 5% level.

I also found that annual earnings were heavily skewed and that college graduates in occupations with higher AI exposure tended to have higher earnings. However, these results don't prove that college or AI caused the differences in salaries.

## Limitations

My research only uses ACS data from 2024, so I can't directly measure how AI has changed earnings over time. Other factors like family background, college major, tuition costs, and work experience could also affect earnings.

The results show associations rather than causal effects.

## Tools

- Python
- pandas and NumPy
- matplotlib
- statsmodels
- Google Colab

## Data Availability

The original Census files are too large to include in this GitHub repository. The datasets can be accessed through the following sources:

- [U.S. Census Bureau — 2024 ACS PUMS](https://www.census.gov/programs-surveys/acs/microdata/access/2024.html)
- [Anthropic Economic Index](https://huggingface.co/datasets/Anthropic/EconomicIndex)
- [New York Fed — College Labor Market](https://www.newyorkfed.org/research/college-labor-market)

## Conclusion

Overall, my research suggests that having a bachelor's degree is associated with higher earnings for both Black and White young adults. However, I can't confidently say the college earnings advantage differs between the two groups. I would like to expand this research by looking at earlier years, different college majors, and how AI exposure might affect future earnings.
