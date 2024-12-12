# 3rd CMI-PB Prediction Challenge

This repository contains code for predicting individual responses to booster vaccinations using machine learning approaches as part of the 3rd CMI-PB Prediction Challenge. The project analyzes various immune system measurements before and after vaccination to predict and rank individual responses. All challenges are attempted using a naive XGBoost model with standard hyperparameters, as well as a more advanced approach with hyperparameter tuning.

## Overview

The challenge involves predicting and ranking individual responses across multiple immune system measurements:

1. **Antibody Response Prediction**
   - Predicting IgG antibody levels against pertussis toxin (PT) at day 14
   - Predicting fold change in IgG-PT levels from day 0 to day 14

2. **Cell Frequency Prediction**  
   - Predicting Monocyte frequency at day 1
   - Predicting fold change in Monocyte frequency from day 0 to day 1

3. **Gene Expression Prediction**
   - Predicting CCL3 gene expression at day 3
   - Predicting fold change in CCL3 expression from day 0 to day 3

4. **T-Cell Response Prediction**
   - Predicting Th1/Th2 (IFN-γ/IL-5) polarization ratio at day 30

## Data

- Harmonized and preprocessed data is available from the CMI-PB Prediction Challenge website [here](https://www.cmi-pb.org/downloads/cmipb_challenge_datasets/current/3rd_challenge/harmonized_and_processed_data/).

## Code

- `challenge.ipynb`: Base implementation using XGBoost with standard hyperparameters
- `challenge_with_hyper.ipynb`: Enhanced implementation with hyperparameter tuning using RandomizedSearchCV
