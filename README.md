# Sampling_comparision

## Introduction to Sampling

Sampling is a valuable technique used to derive insights about a community by studying data from a representative subset, so avoiding the necessity of examining every individual. To rectify the initial dataset imbalance, an oversampling technique was implemented, as there were 763 non-fraudulent cases and only 9 fraudulent cases. This entailed generating supplementary instances of the minority class (fraudulent cases) to match the majority class (non-fraudulent cases), resulting in a harmonized dataset combined into a unified data frame.

## Dataset and Results
1. Dataset --> **Creditcard_data.csv**
2. Result  --> **comparision.csv**

## Various sampling techniques were employed in this study:

1. **Simple Random Sampling:** Involves the random selection of samples from the population.
2. **Systematic Sampling:** Entails regular interval selection after a random start.
3. **Cluster Sampling:** Encompasses randomly selecting clusters from the population.
4. **Stratified Sampling:** Involves the division of the population into subgroups based on specific criteria.
5. **Bootstrap Sampling:** Utilizes resampling with replacement to create multiple samples from the original dataset.
   
Following the generation of five distinct samples using these techniques, five models were applied to each sample. The accuracies of each model for a given sample are summarized in the table below:

| Sampling Technique    | Random Forest | Logistic Regression | Naive Bayes | Decision Trees | KNN    |
|------------------------|---------------|----------------------|-------------|----------------|--------|
| Simple Random Sampling | 0.9870        | 0.8831               | 0.7013      | 0.9610         | 0.8701 |
| Systematic Sampling    | 1.0000        | 0.8926               | 0.7450      | 1.0000         | 0.9329 |
| Cluster Sampling       | 1.0000        | 0.9670               | 1.0000      | 1.0000         | 0.9890 |
| Stratified Sampling    | 1.0000        | 0.9030               | 0.7239      | 0.9925         | 0.9552 |
| Bootstrap Sampling     | 1.0000        | 0.9250               | 0.7500      | 0.9625         | 0.9375 |

In the table above, each row corresponds to a sampling technique, and each column represents the accuracy achieved by each model applied to the respective sample generated using that particular technique.
