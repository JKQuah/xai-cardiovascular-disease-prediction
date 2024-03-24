**Personalized Explainability Requirement Analysis Framework for AI-enabled Systems**

After reviewing recent papers, there is no straightforward way to access the goodness of XAI techniques as mentioned in Cinà et al., 2022. We have to admit that the explanations provided by the systems are subjective. They are highly dependent on the understanding of the receivers regarding their knowledge and educational background. In Explainability Analysis, it generates relevant explanation prototypes with available interpretability techniques. It allows the demonstration of ideas and visualization formats of explanations to stakeholders before the design and implementation phases. In the meantime, the explanations provided by the AI-enabled systems also include technical terms that the non-technical users could not understand such as feature importance, F1 score, or precision score, therefore the specific explanations (i.e., textual, plain-text or visual explanation) should be designed and formulated accordingly to fulfill every stakeholder’s needs and understanding. 


The objective of the prototype is to illustrate each of the intended explanations for each group of stakeholders, allowing the stakeholders to visualize and interact with the simulated version before the developed version is implemented.

**The features used in the heart disease prediction model**
| **No.** | **Feature Name**         | **Type of Feature** | **Feature Data Type** |
| ------- | ------------------------ | ------------------- | --------------------- |
| 1       | Age                      | Objective           | float (years)         |
| 2       | Gender                   | Objective           | categorical code      |
| 3       | BMI                      | Objective           | float                 |
| 4       | Systolic blood pressure  | Examination         | int                   |
| 5       | Diastolic blood pressure | Examination         | int                   |
| 6       | Cholesterol              | Examination         | categorical code      |
| 7       | Glucose                  | Examination         | categorical code      |
| 8       | Smoking                  | Subjective          | categorical code      |
| 9       | Target                   | Target              | categorical code      |

 
**The explainability techniques used to generate respective explanation prototypes**
| **Type of explanation** | **Explainability techniques**               | **Library**           |
| ----------------------- | ------------------------------------------- | --------------------- |
| Plain-fact              | Generalized Linear Rule Model (GLRM) & SHAP | XAI360, Alibi Explain |
| Causal                  | LIME, SHAP                                  | XAI360, Alibi Explain |
| Contrastive             | Comparison of LIME                          | XAI360                |
| Transfactual            | LIME                                        | XAI360                |
| Counterfactual          | DiCE, CounterfactualProto                   | Alibi Explain         |
