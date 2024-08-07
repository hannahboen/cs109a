# Predicting Mental Health with the BRFSS

### Gabe LeBlanc, Hannah Boen, Ethan Tran
### Decemeber 2023

## Overview

This project leverages the Behavioral Risk Factors Surveillance System (BRFSS) to predict mental health outcomes based on demographic factors. The BRFSS, maintained by the CDC, collects data on health-related risk behaviors, chronic health conditions, and the use of preventive services.

## Key Questions

1. Which demographics are associated with variations in mental health?
2. What factors best predict poor mental health days?
3. Do interactions between factors influence mental health outcomes?

## Data and Methodology

### Data Collection & Preparation

- **BRFSS Data (2017-2021)**: Combined and cleaned for uniformity.
- **Income Imputation**: Used 2019 Census data to convert income brackets into continuous variables.
- **Geography Simplification**: Grouped states into 9 Census Bureau divisions and included territories as an extra division.

### Model Development

1. **Unaltered OLS Regression**: Simple but less effective.
2. **Polynomial Regression**: Improved performance with higher computational requirements.
3. **Decision Tree**: Inaccurate due to high cardinality.
4. **Random Forest**: Reduced variance, higher accuracy.
5. **Boosted Tree**: Similar to Random Forest with additional tuning.

## Key Findings

- **High Income**: Associated with fewer poor mental health days.
- **Retirement**: Linked to a decrease in poor mental health days.
- **Unable to Work**: Correlated with the most poor mental health days.
- **Female Gender**: Associated with more poor mental health days.

## Conclusion

Our analysis identified significant demographic predictors of mental health, providing insights for targeted public health interventions.

## Code

The final analysis and model code can be found in the `milestone5.ipynb` notebook.

## Running the Project

1. Clone the repository.
2. Install dependencies.
3. Run `milestone5.ipynb` to reproduce the analysis.

## Authors

- Gabe LeBlanc
- Hannah Boen
- Ethan Tran

## Acknowledgments

Thanks to the CS109A team for their support and to the CDC and US Census Bureau for the data.

