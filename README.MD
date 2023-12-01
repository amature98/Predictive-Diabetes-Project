# DIABETES PREDICTIVE ANALYSIS
## Introduction
This project aims to develop a predictive model for identifying individuals at risk of diabetes based on the PIMA Indian Diabetes Dataset. This dataset includes health-related features such as glucose levels, BMI, and age, providing valuable insights into the factors influencing diabetes.
### Background Information
Diabetes mellitus is a chronic metabolic disorder characterized by elevated blood glucose levels, resulting from insufficient insulin production or the body's inability to effectively utilize insulin. Insulin, a hormone produced by the pancreas, plays a crucial role in regulating blood sugar levels by facilitating the absorption of glucose into cells for energy.
Lifestyle factors, genetics, and obesity contribute to the development of type 2 diabetes. Management may involve lifestyle modifications, oral medications, or insulin therapy.
### Relevance to the Project:
The "Predicting Diabetes" project addresses the significance of early detection of diabetes, particularly type 2 diabetes. Timely identification of individuals at risk allows for preventive measures, lifestyle interventions, and effective management to mitigate complications associated with diabetes.
### Dimensions of Business Understanding
1. Healthcare Impact:
The project aligns with healthcare goals by providing a tool for early prediction of diabetes. Health professionals can use the model's predictions to identify individuals at risk, enabling targeted interventions and personalized healthcare plans.
2. Patient Empowerment:
Individuals at risk of diabetes can benefit from early detection and lifestyle modifications. Communicating the results of the predictive model in an understandable manner empowers patients to make informed decisions about their health.
3.Public Health:
Diabetes has significant public health implications, contributing to a global burden of disease. The project's outcomes can inform public health strategies, emphasizing prevention and reducing the societal impact of diabetes.
4. Business Decision-Making:
Decision-makers in healthcare institutions need to assess the practicality and integration of the predictive model into existing workflows. Understanding the business context ensures that the project aligns with organizational goals and contributes to improved patient outcomes.
### Context and Significance
Understanding the broader context within the healthcare domain, this project addresses the critical need for early diabetes detection. Early identification allows for timely intervention, reducing the risk of complications and improving overall health outcomes. The significance of this project lies in its potential to positively impact healthcare practices and individual well-being.
### Stakeholders
Key stakeholders include healthcare professionals responsible for interpreting model predictions, decision-makers utilizing insights for preventive healthcare strategies, and individuals whose health is being assessed.
1. Healthcare Professionals:
Stakeholders in the healthcare domain will be crucial for understanding the clinical significance of the model's predictions. Their input will guide the interpretability of the model for practical use.
2. Patients and Individuals:
Individuals whose health is being assessed are stakeholders in the context of personal health outcomes. Communication strategies will be developed to convey model predictions in a clear and understandable manner, facilitating informed decision-making.
3. Decision-Makers in Healthcare Institutions:
Those responsible for implementing predictive models in healthcare settings will be consulted to ensure that the model aligns with existing processes and contributes to improved patient outcomes.
4. Insurance Providers:
If applicable, insurance providers may have an interest in understanding the potential impact of the model on healthcare costs and the overall health of insured individuals.
### Success Criteria
Success is defined by achieving specified performance metrics, aligning with the project's primary objective of accurate diabetes prediction. The success criteria are designed to meet the needs of stakeholders and contribute to the overarching goal of improving healthcare outcomes.

## Data Understanding
### Dataset Context
The dataset used for this project is adopted from the Kaggle Pima Indians Diabetes dataset ( <https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database>). This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. The objective of the dataset is to diagnostically predict whether or not a patient has diabetes, based on certain diagnostic measurements included in the dataset. Several constraints were placed on the selection of these instances from a larger database. In particular, all patients here are females at least 21 years old of Pima Indian heritage.
### Dataset Exploration
Exploration of the PIMA Indian Diabetes Dataset involves assessing data structure, identifying missing values and examining feature distributions.
### Data Structure
The dataset consists of:
● One target (dependent) variable, Outcome column, which is a Class variable (0 or 1). 268 of 768 are 1, the others are 0
● Several medical predictor (independent) variables
The independent variables include:
● Pregnancies - The number of pregnancies the patient has had.
● BMI - Body mass index (weight in kg/(height in m)^2):
● Insulin level - 2-Hour serum insulin (mu U/ml):
● Age (years) -
● Glucose - Plasma glucose concentration is a 2 hours in an oral glucose tolerance test
● Blood Pressure - Diastolic blood pressure (mm Hg)
● SkinThickness - Triceps skinfold thickness (mm)
● Diabetes Pedigree Function
### Missing Values
There are no missing values in the dataset

### Preprocessing
Preprocessing steps, such as handling outliers and normalizing numeric features, ensure the dataset is suitable for model training.

### Modeling
## Logistice Regression
The classification_report provides a detailed breakdown of the model's performance. Here's an interpretation of the key metrics:

Precision: The proportion of true positive predictions among all positive predictions. For class 0, precision is 0.81, and for class 1, precision is 0.65. This means that when the model predicts class 0, it is correct 81% of the time, and for class 1, it is correct 65% of the time.

Recall (Sensitivity): The proportion of true positive predictions among all actual positives. For class 0, recall is 0.80, and for class 1, recall is 0.67. This means that the model correctly identifies 80% of all actual class 0 instances and 67% of all actual class 1 instances.

F1-Score: The harmonic mean of precision and recall. It provides a balance between precision and recall. For class 0, the F1-score is 0.81, and for class 1, it is 0.66.

Accuracy: The overall correctness of predictions. The model achieves an accuracy of 0.75, meaning it is correct 75% of the time.

Macro Avg: The average of precision, recall, and F1-score across classes. It's calculated by averaging the metrics for each class. In this case, the macro average precision is 0.73, recall is 0.74, and F1-score is 0.73.

Weighted Avg: Similar to macro average, but it considers the number of instances for each class. It's weighted by the number of instances in each class. In this case, the weighted average precision is 0.76, recall is 0.75, and F1-score is 0.75.
Conclusion
This concise data understanding documentation outlines the project's context, significance, stakeholder considerations, data overview, business requirements, success criteria, and communication plan, laying the foundation for the subsequent stages of the data science project.

### KNN Metrics Analysis
Precision:

Precision for class 0 (No Diabetes): 0.85
Out of all instances predicted as class 0, 85% are truly class 0.
Precision for class 1 (Diabetes): 0.79
Out of all instances predicted as class 1, 79% are truly class 1.

Recall (Sensitivity):
Recall for class 0: 0.90
Out of all actual class 0 instances, the model correctly identifies 90%.
Recall for class 1: 0.70
Out of all actual class 1 instances, the model correctly identifies 70%.

F1-Score:
F1-Score for class 0: 0.87
The harmonic mean of precision and recall for class 0.
F1-Score for class 1: 0.74
The harmonic mean of precision and recall for class 1.

Accuracy:
Overall correctness of predictions: 0.83
The model is correct 83% of the time across both classes.
Macro Avg:
The average of precision, recall, and F1-score across classes.
Macro average precision: 0.82, recall: 0.80, F1-score: 0.81
Weighted Avg:
Similar to the macro average, but it considers the number of instances for each class.
Weighted average precision: 0.83, recall: 0.83, F1-score: 0.83
Interpretation:

The model performs well in terms of precision, recall, and F1-score for both classes, indicating a balanced performance.
Class 0 (No Diabetes) has higher precision, recall, and F1-score than class 1 (Diabetes).
The weighted average takes into account the class imbalance, providing an overall performance metric for the model.

The ROC AUC score of 0.902 indicates that your binary classification model has a very good ability to discriminate between the two classes. It suggests that the model is effective at assigning higher predicted probabilities to positive instances compared to negative instances, leading to a strong separation between the positive and negative classes on the ROC curve.

