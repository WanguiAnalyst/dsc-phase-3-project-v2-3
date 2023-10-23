
#  Customer Churn Prediction Analysis for Telco

![telecom churn Intro](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/f71f3f97-4fea-474e-b5b9-6881354a3271)

## Project Overview
Business Problem:
Customer churn, the departure of customers, impacts revenue and profitability. 

The project aims to identify reasons for churn and develop strategies for its reduction in the telecom industry to enhance business performance.

## Business and Data Understanding
The project uses the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, which encompasses several stages:

- Business understanding
- Data Understanding
- Data preparation
- Modeling
- Evaluation
- Deployment

### Stakeholder Audience

The key stakeholders for this project are the management and decision-makers of the telecommunications company. They would be interested in understanding the factors contributing to customer churn and exploring effective strategies to reduce it, ultimately leading to improved revenue and profitability.

### Dataset Overview
The dataset used in this project contains information about 3,333 customers of the telecommunications company, spanning 21 columns. These columns cover various details, including:

- Customer's state
- Account length
- Phone number
- International plan subscription
- Voicemail plan subscription
- Number of voicemail messages
- Day, evening, and night usage details (minutes, calls, charges)
- International usage details (minutes, calls, charges)
- Number of customer service calls
- Churn status (whether the customer has churned or not)

### Data Preprocessing

Checked for: 
* Missing data
* Duplicates
 
Target Variable:
* Churn
  
Dropped Features that were not 
significant such as :
* Phone numbers


### EDA

![Numerical Features Distribution](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/5fe8ee12-35e9-4f00-a26a-0d30886a6660)
![Correlation matrix](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/0f617f64-3136-409e-93fb-eeb98f6b6a56)
![Area code and Churn](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/040b78a4-489d-4af7-a4d9-ab73c1278e55)
![Top 10 States vs Churn](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/5e3d50eb-559c-4f77-bcfa-e91b6195083e)
![Categorical data](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/535362e1-d8a7-4acd-917e-f87655c3e0fd)
![Account length and churn](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/77c0b80d-f7b9-4ef4-bc16-28424b44e250)
![Feature importance](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/66ae9772-af97-45aa-8810-23705536868f)

## Modeling

The modeling phase involved the construction and assessment of various predictive models. 

The process began with a basic logistic regression model and progressed towards more complex models, Decision Tree and Random Forest.

## Evaluation

Performance evaluation of the models was conducted using various metrics, including accuracy, precision, recall, and F1-score.

![Measures of model prediction](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/95062118-ca21-48eb-871e-26c18f1dc1f0)

![Model Results](https://github.com/WanguiAnalyst/dsc-phase-3-project-v2-3/assets/125726694/0f777375-c611-4305-abf1-3a6db820cc7b)

Though Decision Tree Model outperformed the other two models, we will pick the 
Random Forest Model which has the highest recall and aligns better with our 
business requirements as it minimizes the risk of losing customers who were 
incorrectly classified.

## Recommendations

Based on the analysis, several actionable insights were derived that can help the business reduce customer churn:

* Focus on improving customer service as it's a major determinant of customer satisfaction.
* Engage with customers who have high daily usage, as they are more likely to churn.
* Consider special plans or offers for long-term customers and regions with high churn rates to incentivize loyalty.
  
## Conclusion

In summary, our analysis unveils limitations in feature relevance, model selection, potential external influences, and the risk of overfitting. Despite these constraints, I derived actionable recommendations, emphasizing improvements in customer service, engagement with high-usage customers, and the implementation of loyalty incentives to mitigate churn. 

It's imperative for businesses to recognize and leverage these insights to enhance customer retention and drive profitability.

Additionally, I underscore the importance of addressing states or area codes with high churn rates, as these regions may require tailored strategies for effective churn reduction. 
  
## Limitations

* **Feature Relevance:** 
  * Not all dataset features were impactful for predicting churn, leading to potential model inefficiencies.
  * Lack of detailed information on states and area codes prevented further in-depth

* **Modeling:**
  * Model Selection: Despite using Logistic Regression, the focus was on tree-based models. Exploring models like gradient boosting or neural networks might enhance performance.
  * Further research and analysis, considering additional data sources and alternative modeling approaches, are recommended to enhance our understanding and strategy for reducing customer churn effectively.
* **External Factors:**
  * Temporal Changes: The data might exhibit unnoticed trends over time, affecting the analysis.
  * Bias Concerns: Potential biases, such as geographic or demographic, in the dataset could skew results.
* **Generalization:**
  * Overfitting Risk: Models, especially complex ones like Random Forest, might overfit, necessitating robust validation and regularization.
