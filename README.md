# Interpretable-Causal-Inference



I use The dame-flame package, the package offers efficient,  easy-to-use  implementations  of  the  DAME  andFLAME algorithms, allowing users to perform fast, interpretable matching for causal infer-ence for observational data with discrete covariates. The package uses 2 different algos to generate the matches:

- FLAME “Fast Large-Scale Almost Matching Exactly” algorithm
- DAME “Dynamic Almost Matching Exactly” algorithm

The advantage of matchingis  is that  it  reduces  bias  of  treatment  effect  estimates,  and  permits  interpretable  analyses that are easier to troubleshoot than other types of analysis for observational causal studies.

## Notions: Cause - effect - treatment - control 

## Matching based analysis for observational causal studies

Matching methods are heavily used in the social and health sciences due to their interpretability. We aim to create the highest possible quality of treatment-control matches for categorical data in the potential outcomes framework. The method proposed in this work aims to match units on a weighted Hamming distance, taking into account the relative importance of the covariates; the algorithm aims to match units on as many relevant variables as possible. To do this, the algorithm creates a hierarchy of covariate combinations on which to match (similar to downward closure), in the process solving an optimization problem for each unit in order to construct the optimal matches. The algorithm uses a single dynamic program to solve all of the units’ optimization problems simultaneously. Notable advantages of our method over existing matching procedures are its high-quality interpretable matches, versatility in handling different data distributions that may have irrelevant variables, and ability to handle missing data by matching on as many available covariates as possible. 
