# Predictive Modeling of Customer Churn in Streaming Services  
Floriand Beshku | 2026  

This project demonstrates how data can be used to improve customer retention decisions by replacing intuition-based strategies with an objective, data-driven approach. Rather than relying on broad assumptions, this analysis predicts which users are most likely to cancel their subscription and explains which behaviors meaningfully influence that decision.

---

## Business Problem

In many subscription-based businesses, retention decisions are driven by intuition, leading to inefficient use of resources and missed opportunities to prevent churn. Companies often apply generic retention strategies without identifying which users are truly at risk.

- **Identify At-Risk Users:** Detect which customers are most likely to churn before they cancel.  
- **Reduce Inefficient Retention Efforts:** Avoid targeting users who are unlikely to leave.  
- **Improve Retention Outcomes:** Focus on high-impact behaviors that drive customer decisions.  

---

## Technical Stack

- **Language:** Python  
- **Environment:** Anaconda / Jupyter Notebook  
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn  
- **Modeling:** Decision Tree Classification  

---

## Methodology & Workflow

A structured data science workflow was followed to ensure reliability and interpretability:

- **Data Preparation:** Cleaned a dataset of 1,000 streaming users, removed identifiers, and encoded categorical variables.  
- **Data Partitioning:** Split the data into Training (50%), Validation (30%), and Test (20%) sets using stratified sampling.  
- **Predictive Modeling:** Developed a Decision Tree model to classify churn risk based on user behavior and subscription characteristics.  
- **Model Tuning:** Applied hyperparameter tuning to control tree complexity and improve generalization.  
- **Model Evaluation:** Assessed performance using confusion matrices, accuracy, precision, recall, and F1-score.  
- **Interpretation:** Extracted decision rules and feature importance to generate actionable business insights.  

---

## Key Results & Business Insights

The analysis identified several key drivers of customer churn:

- **Content Consumption (Most Important):**  
  Users with low content views are significantly more likely to churn, while highly engaged users tend to remain subscribed.  

- **Subscription Price (Conditional Effect):**  
  Higher monthly fees increase churn risk primarily when engagement is low.  

- **Customer Tenure:**  
  Long-term users are more loyal and less likely to cancel.  

- **Inactivity Patterns:**  
  Users who stop engaging with the platform show increased churn risk, although engagement level is a stronger predictor than inactivity alone.  

- **Engagement Dominates Price Sensitivity:**  
  Highly engaged users remain subscribed even at higher price levels, indicating strong perceived value.  

---

## Model Performance

The tuned decision tree achieved balanced and realistic performance:

- **Accuracy:** ~79%  
- **Precision:** ~57%  
- **Recall:** ~50%  
- **F1-Score:** ~53%  

The model capture a meaningful portion of at-risk users while maintaining reasonable precision.

---

## Practical Application

The decision tree model provides clear, rule-based insights that can be directly applied in business settings:

- **Targeted Retention Campaigns:** Identify and prioritize high-risk users for intervention.  
- **Personalized Recommendations:** Increase engagement for low-activity users.  
- **Pricing Strategy Optimization:** Adjust pricing strategies for low-engagement segments.  
- **Customer Segmentation:** Group users based on behavior and churn risk for better decision-making.  

Unlike black-box models, this approach is transparent and easy to interpret, making it suitable for real-world deployment in marketing, product, and customer experience teams.

---

## Key Takeaway

Customer engagement is the strongest driver of retention. Users who actively consume content are far less likely to churn, while low engagement combined with higher pricing creates the highest risk segments.  

The decision tree model provides a practical and interpretable framework for identifying these patterns and supporting data-driven retention strategies.
