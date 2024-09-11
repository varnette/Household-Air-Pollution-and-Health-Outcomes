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

## Discussion

The findings highlight the importance of targeted public health interventions aimed at reducing health disparities in low-wealth regions. Improving access to electricity and promoting cleaner cooking fuels are actionable interventions that can reduce disease burden. The analysis underscores the need for more granular data to refine models and provide more specific recommendations for public health strategies.

## Conclusion

This analysis emphasizes the critical need for targeted public health interventions to mitigate poor health outcomes related to environmental and indoor air pollution, particularly in low-wealth regions. By focusing on improving household conditions and expanding access to clean energy sources, stakeholders can address the underlying social determinants of health and foster more equitable health environments for all populations.
