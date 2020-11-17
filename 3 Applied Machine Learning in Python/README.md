# Course Content:
- Describe how machine learning is different than descriptive statistics;
- Explain different approaches for creating predictive models;
- Create and evaluate data clusters;
- Build features that meet analysis needs.

## Work: Machine Learning Classification Task to Predict whether a Pregnant Women will make a Cesarian or not

This works aims to predict a Cesarian based on some attributes, presented above. The dataset, which can be found here, is from the UCI repository, and is a classification problem, univariate with 80 instances i.e. samples, and 5 attributes.

#### Attribute Information:
- Age: [22,26,28,27,32,36,33,23,20,29,25,37,24,18,30,40,31,19,21,35,17,38]
- Delivery number: [1,2,3,4]
- Delivery time: [0,1,2] -> 0 = timely , 1 = premature , 2 = latecomer
- Blood of Pressure: [2,1,0] -> 0 = low , 1 = normal , 2 = high
- Heart Problem: [1,0] -> 0 = apt, 1 = inept
- Cesarian: [0,1] -> 0 = No, 1 = Yes

This work approaches Initial Data Analysis (IDA), Exploratory Data Analysis (EDA), Feature Engineering, and Machine Learning Algorithms (linear classifiers and tree-based classifiers), as well as SHAP (*SHapley Additive exPlanations*) in order to explain the model's outputs.
