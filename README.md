<h1 style="text-align:center;">PREDICTION MODELS FOR CUSTOMER CHURN IN SYRIATEL TELECOMMUNICATIONS COMPANY</h1>

<div style="text-align:center;">
  <img src="Images/Telcos Business Infrastructure.jpg" alt="Telcos Business" width="600" height="500">
</div>

<h1 style="text-align:center;">OVERVIEW OF THE PROJECT</h1>
The project endeavors to develop a predictive model for customer churn, with the primary objective of identifying customers who may be inclined to discontinue services. Stakeholders within the telecommunications industry, including marketing and sales teams, customer service departments, and upper management, stand to benefit substantially from the outcomes of the project. The project scope includes the development and evaluation of predictive models with the potential to significantly enhance customer retention and overall profitability of telcos.

<h1 style="text-align:center;">BUSINESS UNDERSTANDING</h1>
SyriaTel, a leading telecommunications firm, grapples with a customer 'churn' problem. The churn problem poses revenue and reputation risks to the company. To address this, SyriaTel seeks predictive insights and a reliable classifier model to anticipate customer churn effectively.


Specific Objectives:

- To develop a binary classification model to predict whether a client will imminently terminate their relationship with SyriaTel.
- Identify the factors influencing customer churn.
- Select the optimal model for forecasting customer churn.

<h1 style="text-align:center;">DATA UNDERSTANDING</h1>
The dataset originates from SyriaTel Telecommunication company and was obtained from Kaggle (link: https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset/data). It comprises 21 columns and 3333 rows. The columns have various attributes related to customer demographics, service usage, and churn behavior. The rows correspond to a recorded customer. The dataset encompasses both continuous and categorical variables. The target variable identified is "churn," with the remaining variables serving as predictors, excluding "state" and "phone number".

<h1 style="text-align:center;">DATA PREPARATION</h1>
This analysis employs Exploratory Data Analysis on the SyriaTel dataset to check for patterns or insights useful for predicting churn. Some steps of EDA include Data Visualization and Correlation Analysis.

- Data Visualization: Visualizations such as histograms and bar charts are useful to be able to understand the distribution and relationships between different variables in the SyriaTel dataset.

<div style="text-align:center;">
  <img src="Images/Distribution of Churn in SyriaTel.png" alt="Distribution of Churn" width="500" height="400">
</div>

- Correlation Analysis was used as a Feature Importance/Selection techinique to select the most influential features in predicting 'churn'.

- Data Preprocessing was employed to create Graphs and Visualization used to analyse data to be used for Modeling. 

<div style="text-align:center;">
  <img src="Images/Distribution of features in SyriaTel Data.png" alt="Distribution of Features" width="500" height="400">
</div>

<h1 style="text-align:center;">MODELING</h1>

The data was split into the training and test datasets. The training dataset served as the foundation for model training endeavors to fit the models. The test subset functioned as an independent validation mechanism to assess the models' predictive capabilities. A Baseline Logistic Regression Model was developed. More-complex models such as Random Forest Model, XGBoost Model and a Tuned Random Forest Model
were developed.

<h1 style="text-align:center;">EVALUATION</h1>

 Among the models evaluated, XGBoost demonstrates superior performance in terms of accuracy, precision, recall, F1 score, and ROC AUC score.
 XGBoost Model achieved an accuracy of 96.4%, a precision of 95.3%. The XGBoost Model also has the best overall performance in terms of churn prediction i.e True positives (TP). It has the highest number of true positives (81) and true negatives (562) with relatively low false positives (4) and false negatives (20).
 Evaluating the Models based on the ROC AUC (Receiver Operating Characteristic - Area Under the Curve) metric:

 - The Baseline Model using Logistic Regression achieved an ROC AUC score of 0.8760. This indicates that the model performs reasonably well in distinguishing between the positive and negative classes.

- The More-complex Model using Random Forest achieved an ROC AUC score of 0.9249. Compared to the Baseline Model, the Random Forest model shows an improvement in performance, as indicated by the higher ROC AUC score.

- The XGBoost Model achieved an ROC AUC score of 0.9294. This model shows a further improvement in performance compared to both the Baseline Model and the More-complex Model using Random Forest.

- The Tuned Random Forest Model achieved an ROC AUC score of 0.9222. Despite being tuned, this model's performance, as measured by the ROC AUC score, is slightly lower than the XGBoost Model but still higher than the Baseline Model and the More-complex Random Forest Model.

<div style="text-align:center;">
  <img src="Images/Models ROC curve.png" alt="ROC Curves" width="500" height="400">
</div>

<h1 style="text-align:center;">CONCLUSION</h1>

SyriaTel faces a significant challenge with customer churn, which poses both financial and reputational risks. Through comprehensive analysis and modeling, it's evident that predictive analytics can offer valuable insights into customer behavior and aid in proactive churn management. Among the models evaluated, XGBoost demonstrates superior performance in terms of accuracy, precision, recall, F1 score, and ROC AUC. Key features such as international plan status, customer service calls, and total day minutes emerge as crucial predictors of churn. Moving forward, SyriaTel should focus on implementing the recommendations oulined here.

<h3 style="text-align:center;">Recommendations</h3>

- **Implement targeted retention strategies: Utilize predictive insights to identify high-risk customers and deploy personalized retention tactics, such as tailored offers or proactive customer service interventions.**

- **Enhance customer experience: Invest in improving service quality and addressing pain points identified through customer feedback and analytics to foster loyalty and reduce churn.**

- **Continuously monitor and adapt: Regularly assess model performance and customer trends to refine predictive models and strategies, ensuring relevance and effectiveness over time.**

<h3 style="text-align:center;">Next Steps</h3>

- **Conduct deeper analysis: Explore additional data sources and factors influencing churn, such as customer demographics or usage patterns, to enhance predictive accuracy and identify new insights.**

- **Address model limitations: Address potential biases or limitations in the dataset, such as data imbalance or missing features , through data preprocessing techniques and model refinement to improve predictive performance and reliability.**

## Repository Guide

The datasets used can be found [here](Data)

The notebook can be found [here](SyriaTel_Customer_Churn_EDA.ipynb)

The presentation can be found [here](<SyriaTel Customer Churn Presentation.pdf>)
