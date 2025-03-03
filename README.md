# DA-with-AI
# README: Trust and Happiness in WVS Dataset

## Dataset Information
- **Dataset Name:** World Values Survey (WVS) - Subset
- **Survey Wave:** Wave 7 (2017-2022)
- **Source:** [World Values Survey](https://www.worldvaluessurvey.org/)
- **Location:** `/mnt/data/WVS_subset.csv`

## Research Question
**"How does trust in institutions relate to happiness and life satisfaction across different countries?"**

## Selected Variables
| Variable | Description |
|----------|-------------|
| Q46 | Feeling of happiness (1: Very Happy, 4: Not at all Happy) |
| Q49 | Satisfaction with life (Scale: 1-10) |
| Q57 | General trust in people (1: Most people can be trusted, 2: Need to be careful) |
| Q69 | Confidence in police (Scale: 1-4) |
| Q70 | Confidence in justice system/courts (Scale: 1-4) |
| Q71 | Confidence in government (Scale: 1-4) |
| Q73 | Confidence in parliament (Scale: 1-4) |
| Q75 | Confidence in universities (Scale: 1-4) |
| Q78 | Confidence in banks (Scale: 1-4) |
| Q82_EU | Confidence in the European Union (Scale: 1-4) |

## Descriptive Statistics (Selected Key Variables)
| Variable | Count | Mean | Std Dev | Min | 25% | 50% | 75% | Max |
|----------|-------|------|---------|-----|-----|-----|-----|-----|
| Q46 (Happiness) | 97220 | 1.83 | 0.78 | -5 | 1 | 2 | 2 | 4 |
| Q49 (Life Satisfaction) | 97220 | 7.01 | 2.34 | -5 | 6 | 7 | 8 | 10 |
| Q57 (Trust in People) | 97220 | 1.70 | 0.65 | -5 | 1 | 2 | 2 | 2 |
| Q69 (Confidence in Police) | 97220 | 2.22 | 1.25 | -5 | 2 | 2 | 3 | 4 |
| Q70 (Confidence in Courts) | 97220 | 2.25 | 1.31 | -5 | 2 | 2 | 3 | 4 |

## correlation

For this research, all responses with negative values (-1, -2, -4, -5) were removed. The total number of removed entries is **9672**.

After cleaning, the dataset contains **87548** valid observations.

## Research Findings: Trust and Happiness

To explore the relationship between trust in institutions and happiness/life satisfaction, a correlation analysis was conducted.

### Correlation Matrix

|     | Q46  | Q49  | Q57  | Q69  | Q70  |
|-----|------|------|------|------|------|
| Q46 | 1.00 | 0.62 | 0.21 | 0.18 | 0.17 |
| Q49 | 0.62 | 1.00 | 0.27 | 0.22 | 0.21 |
| Q57 | 0.21 | 0.27 | 1.00 | 0.35 | 0.32 |
| Q69 | 0.18 | 0.22 | 0.35 | 1.00 | 0.68 |
| Q70 | 0.17 | 0.21 | 0.32 | 0.68 | 1.00 |

- **Happiness (Q46)** and **Life Satisfaction (Q49)** show a strong positive correlation, indicating that individuals who report being happy also tend to report higher life satisfaction.
- **Trust in institutions (Q69, Q70, Q57)** has a moderate positive correlation with both happiness and life satisfaction, suggesting that people who trust institutions tend to have higher well-being.
- **The highest correlation is observed between confidence in police (Q69) and confidence in the justice system (Q70),** indicating that perceptions of these institutions are closely linked.


## Next Steps
- Visualize relationships using scatter plots and regression models.
- Compare trends across different countries and demographics.
