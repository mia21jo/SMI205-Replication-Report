---

# "SMI205-Replication-Report: COVID-19 Impact on Mental Health"

---

## Project Overview

This project replicates and extends the study titled "COVID-19 Impacts on Mental Health" by Cui et al. (2022). The original study investigated the impact of the COVID-19 pandemic on mental health, focusing on factors like employment income loss, delayed or unmet medical care needs, housing insecurity, and having children enrolled in school. This replication project specifically explores the moderating effect of living arrangements (marital status) on the relationship between employment income loss and mental health.

## Objective

To determine whether the impact of employment income loss on mental health during the COVID-19 pandemic varies based on an individual's living arrangements (living alone or with others). 

-*Original Study:* Cui, J. et al. (2022). COVID-19 Impact on Mental Health. BMC Medical Research Methodology.

-*Replication Extension:* Examines the moderating effect of living arrangement on the relationship between employment income loss and mental health.

-*Hypothesis:* The loss of employment income will have a stronger impact on the mental health of individuals living alone compared to those living with others during the pandemic.

## Project Documentation 

-*README.md:* this file
-*SMI205_Preregistration_form:* preregistration document for this replication extension

## Dataset

-*Source:* Household Pulse Survey Public Use File (PUF)
- *Provider:* U.S. Census Bureau
- *Access:* [Census.gov](https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html)

### Data Preparation

1. *Data Cleaning:*
   - Remove participants with missing values for key variables (employment income loss, marital status, mental health, race, age, education).
   - Handle outliers using visual inspection methods like box plots and scatterplots.
   
2. *Variable Definitions:*
   - *Dependent Variable:* Mental Health (1 = yes, 0 = no)
   - *Independent Variable:* Employment Income Loss (1 = yes, 2 = no)
   - *Moderating Variable:* Marital Status (1 = now married, 2 = widowed, 3 = divorced, 4 = separated, 5 = never married)
   - *Control Variables:* Race and Education
   
### Data Analysis

*Statistical Modeling:*
   - Use logistic regression with interaction terms to test the hypothesis.
   - Model specification: Mental Health ~ Employment Income Loss * Marital Status + Control Variables
   - Interaction terms included to assess the moderating effect of marital status.

### My Environment

```{r}
sessionInfo()
```

