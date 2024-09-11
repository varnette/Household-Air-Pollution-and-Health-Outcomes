## Targeting Interventions: Bridging the Data Gap in Household Air Pollution and Health Outcomes at the Subnational Level
  
[View full report here](https://docs.google.com/document/d/1ffMM9habn9fEqMWWX90mDZaVvzD_LI-i2kjPFsOF9NQ/edit?usp=sharing)

## Executive Summary 📊

This analysis aims to address the significant gap in region-specific health outcome data in developing countries, particularly concerning the impacts of household air pollution. Using data from the **World Health Organization (WHO)** and the **Global Data Lab**, a predictive model was developed utilizing variables such as the **International Wealth Index (IWI)**, access to electricity, types of cooking fuels, and other socioeconomic indicators. The study extends national-level predictions to regional levels where data is currently scarce.

The findings suggest that **low-wealth regions**, especially in **Sub-Saharan Africa and South Asia**, are associated with disproportionately high rates of adverse health outcomes. These outcomes appear to be linked to poor household conditions, such as reliance on biomass for cooking and limited access to electricity. The analysis indicates that **targeted interventions**, including promoting cleaner cooking fuels and improving access to electricity, may help reduce health disparities in these areas.

Using **random forest regression** and **cluster analysis**, the study identifies key variables most strongly associated with poor health outcomes, such as natural flooring, electricity access, and cooking fuel type. The A/B tests conducted further illustrate the potential impact of improving these household conditions on reducing disease burden, particularly for **Chronic Obstructive Pulmonary Disease (COPD)**.

The report concludes that enhancing data granularity and tailoring public health strategies to address specific regional needs are crucial steps toward mitigating the health disparities exacerbated by environmental factors in low-wealth regions. **Public health officials, researchers, and policymakers** should prioritize interventions focused on improving household environments to achieve more equitable health outcomes.

## Introduction

Household air pollution and deaths attributable to environmental factors remain significant global challenges, disproportionately affecting people in developing countries. The World Health Organization (WHO) provides national-level data on health outcomes, such as disability-adjusted life years (DALYs) and deaths attributable to the environment. However, there is a lack of data regarding air pollutant concentrations and associated health outcomes at the subnational level, particularly in developing countries. To fill this gap, the Global Data Lab offers extensive subnational data on housing quality, living standards, and socioeconomic conditions.

Given the considerable variations in living standards and socioeconomic status across regions, there is a need for health outcome data not just at the national level but also at the subnational level to effectively target public health interventions. This analysis investigates the relationships between national health outcome data and various socioeconomic and environmental variables, including IWI, poverty levels, the percentage of households using wood for cooking, the percentage of households with natural flooring, the Gini coefficient, and urbanization rates.

## Analytical Approach

The analysis uses random forest regression to develop a model predicting health outcomes at the regional level. It evaluates the impact of changes in housing quality and wealth through A/B testing and uses K-Means clustering to identify countries and regions with similar characteristics influencing their susceptibility to poor health outcomes. This approach aims to pinpoint variables most strongly associated with adverse health outcomes, such as access to electricity and types of cooking fuel, thereby guiding stakeholders in prioritizing public health interventions.

## Results

The model demonstrates strong predictive performance across various health outcomes related to household air pollution and environmental factors. Key metrics, including Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), R-squared, and Average % Accuracy, were evaluated for different dependent variables. The analysis identified that household conditions, such as cooking fuel type and electricity access, significantly impact health outcomes, particularly in relation to Chronic Obstructive Pulmonary Disease (COPD).

A/B tests confirmed that eliminating the use of wood for cooking or improving household conditions like flooring can significantly reduce COPD-related DALYs. Clustering analysis further revealed that low-wealth groups experience worse health outcomes compared to moderate and high-wealth groups, even when exposed to similar levels of environmental pollutants like PM2.5.A/B tests confirmed that eliminating the use of wood for cooking or improving household conditions like flooring can significantly reduce COPD-related DALYs. Clustering analysis identified three primary groups—low wealth, moderate wealth, and high wealth—based on existing national data. These groups exhibited clear differences in health outcomes, with low-wealth groups experiencing significantly worse health outcomes compared to moderate and high-wealth groups, even when exposed to similar levels of environmental pollutants like PM2.5. This clustering further emphasizes the disparities in health conditions and highlights the need for targeted interventions in low-wealth regions.  The following 3 charts pertain to existing national data analyzed during the project. 

![Clusters national pic ](https://github.com/user-attachments/assets/f92c9eaa-69e7-459d-b072-92092396e225)

![bigger chart health outcomes](https://github.com/user-attachments/assets/7d8e70cf-00de-4fe9-be93-2145cfadbc2d)

![health by type pic](https://github.com/user-attachments/assets/2eac2294-c72e-4897-8b9b-caf4aa2f01bd)

Performance metrics for the random forest are noted below, followed by predicted health outcomes at the subnational level.

| Dependent Variable (Age Standardized, per 100,000 Population)                        | Mean Absolute Error | Mean Squared Error | Root Mean Squared Error | R-squared | Average % Accuracy |
|--------------------------------------------------------------------------------------|---------------------|--------------------|--------------------------|-----------|---------------------|
| Death rate attributable to household air pollution - Total                           | 11.23               | 203.72             | 14.27                    | 0.84      | 87.19               |
| Death rate attributable to household air pollution - COPD                            | 0.17                | 0.05               | 0.23                     | 0.80      | 93.27               |
| Death rate attributable to household air pollution - Ischaemic heart disease         | 4.84                | 37.16              | 6.10                     | 0.73      | 84.29               |
| Death rate attributable to household air pollution - Lower respiratory Infection     | 0.14                | 0.04               | 0.21                     | 0.86      | 95.62               |
| Death rate attributable to household air pollution - Stroke                          | 3.26                | 18.03              | 4.25                     | 0.92      | 85.94               |
| Death rate attributable to household air pollution - Trachea, bronchus, lung cancers | 0.18                | 0.06               | 0.23                     | 0.84      | 78.89               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Total| 259.91              | 1126418.26         | 355.55                   | 0.88      | 87.87               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Lower respiratory infection | 167.65             | 35780.58           | 189.16                   | 0.90      | 81.56               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Trachea, bronchus, lung cancer | 0.28             | 0.14               | 0.37                     | 0.81      | 91.65               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Cataracts | 4.61             | 35.89              | 5.99                     | 0.83      | 77.95               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Ischaemic heart disease | 104.97            | 18608.45           | 136.41                   | 0.74      | 84.36               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - Stroke | 82.41              | 11686.19           | 108.10                   | 0.91      | 84.11               |
| Disability Adjusted Life Years (DALYs) attributable to household air pollution - COPD | 0.16                | 0.05               | 0.22                     | 0.81      | 97.26               |
| Death attributable to the environment - Total                                        | 16.14               | 405.28             | 20.13                    | 0.90      | 92.25               |
| Death attributable to the environment - Infectious, parasitic, neonatal, and nutritional | 14.17            | 287.57             | 16.96                    | 0.85      | 74.04               |
| Death attributable to the environment - Injuries                                      | 4.63                | 37.33              | 6.11                     | 0.83      | 88.27               |
| Death attributable to the environment - Noncommunicable Diseases                      | 8.61                | 119.68             | 10.94                    | 0.88      | 92.95               |


![subnat predict](https://github.com/user-attachments/assets/13b75bbe-1745-4b5b-a8ea-39cb8403de07)

![subnat by condition](https://github.com/user-attachments/assets/cde964bf-46b1-4e58-a199-32c3b01ff12d)

## Discussion

The findings highlight the importance of targeted public health interventions aimed at reducing health disparities in low-wealth regions. Improving access to electricity and promoting cleaner cooking fuels are actionable interventions that can reduce disease burden. The analysis underscores the need for more granular data to refine models and provide more specific recommendations for public health strategies.

## Conclusion

This analysis emphasizes the critical need for targeted public health interventions to mitigate poor health outcomes related to environmental and indoor air pollution, particularly in low-wealth regions. By focusing on improving household conditions and expanding access to clean energy sources, stakeholders can address the underlying social determinants of health and foster more equitable health environments for all populations.
