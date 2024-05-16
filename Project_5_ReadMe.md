# Oil_Spill_Analysis_and_Resource_Optimization

## Introduction
This project aims to analyze historical oil spill data, develop predictive models to estimate the total cost of dealing with spills, and utilize these predictions to inform resource allocation strategies for spill response efforts.

## Part 1: Spatial Clustering
- **Challenges:** Dealing with missing values, particularly in geospatial data, posed challenges during visualization. Additionally, understanding the relationships between different features required careful analysis.
- **Resolutions:** Missing values were handled by either imputation or exclusion, depending on the context. Visualization challenges were addressed by using appropriate libraries and techniques, such as geospatial plotting tools.
- **Assumptions:** I assumed that missing geospatial data could be safely excluded from analysis without significantly affecting overall insights.
- **Conclusions:** Geospatial analysis revealed hotspots of oil spill occurrences, while correlation analysis highlighted key factors influencing spill occurrences.
- **Evaluation Results:** Silhouette Score: 0.49832848637333427
Davies-Bouldin Index: 0.6137532037813581
Calinski-Harabasz Index: 2296.5258676329995
Inertia: 149319.92614824662


## Part 2: Predictive Modeling
- **Challenges:** Model selection and hyperparameter tuning required experimentation and careful evaluation to achieve optimal performance. Dealing with categorical variables and encoding them appropriately was also a challenge.
- **Resolutions:** I experimented with multiple regression models, including Gradient Boosting, and fine-tuned hyperparameters using techniques like grid search. Categorical variables were encoded using one-hot encoding to ensure compatibility with the models.
- **Assumptions:** I assumed that the relationships between features and spill costs were adequately captured by the chosen models and that the encoded categorical variables effectively represented the underlying information.
- **Conclusions:** The Gradient Boosting model showed promising performance in predicting spill costs, providing valuable insights for decision-making.
- **Evaluation Results:** Mean Squared Error: 50353792187182.9
R^2 Score: 0.4608734624137527

## Part 3: Resource Allocation Strategy
- **Challenges:** Developing a resource allocation strategy based on predictive models required careful consideration of various factors, including model uncertainty and practical feasibility.
- **Resolutions:** While no specific resource allocation strategy was developed, we discussed the potential use of predictive models to inform decision-making in spill response efforts. This involved exploring the model's utility and limitations in real-world applications.
- **Assumptions:** I assumed that the predictive models could provide useful insights into the expected costs of spill response efforts and that stakeholders would be receptive to incorporating these insights into resource allocation decisions.
- **Conclusions:** The predictive models can serve as valuable tools for optimizing resource allocation in spill response efforts, improving efficiency, and reducing costs.

## Dataset
The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/usdot/pipeline-accidents/data). It contains information about historical oil spills, including details about spill location, causes, costs, and other relevant factors.
