# Data Scientist Nanodegree - Project Part 1

## Motivation

The aim of this project is to apply the CRISP-DM process for data analysis to the Kaggle Airbnb Seattle Dataset within the Part 1 Project of the Udacity Data Scientist Nanodegree.

You can find the dataset in the repository or in the following Kaggle link:

https://www.kaggle.com/airbnb/seattle

The CRISP-DM process consists of the following parts, which are replicated in the attached notebook:

1. Business Understanding 
2. Data Understanding
3. Data Preparation 
4. Modeling
5. Evaluation
6. Deployment

For the first point, I'm answering the following questions:

- How does the availability varies during the year in Seattle?
- Which are the neighbourhoods (zip codes) with better price/review ratio?
- Can we predict the prices of the apartments?

## Used Packages

- Python        3.7.0
- Pandas        1.0.3
- Numpy         1.15.1
- Matplotlib    3.2.1
- Sklearn       0.24.1

## Key Insights and results

The complete analysis can be found in the Notebook

**How does the availability varies during the year in Seattle?**

Mean price across the year:

![Image: Mean price across the year ](graphs/mean_price.png)

and the corresponding availability:

![Image: Availability across the year ](graphs/availability.png)

**Which are the neighbourhoods (zip codes) with better price/review ratio?**

| Neighbourhood | Zipcode | Ratio |
| --- | --- | --- |
| Unknown | 98108 | 0.149 |
| Maple Leaf | 98125 | 0.138 |
| South Delridge | 98106 | 0.137 |
| The Junction | 98118 | 0.136 |
| Bitter Lake | 98133 | 0.134 |
| Crown Hill | 98177 | 0.132 |
| Arbor Heights | 98146 | 0.12 |
| Green Lake | 98115 | 0.119 |
| Wallingford | 98105 | 0.118 |

**Can we predict the prices of the apartments?**

|   | RSME | R2-score |
| --- | --- | --- |
| Linear regression | 57.909940 | 0.560165 |
| Linear regression with opt. features | 64.910752 | 0.447392 |
| Random forest | 59.608005| 0.533992 |
| Ensemble | 56.735968| 0.577817 |



