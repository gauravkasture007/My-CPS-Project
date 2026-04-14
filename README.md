ConnectTel Advanced Churn Prediction Strategy 📡💡

🏢 Business Context

ConnectTel, a leading telecommunications provider, is facing a surge in customer churn due to intense market competition. The objective of this project is to move from reactive customer service to proactive retention by identifying high-risk customers before they leave.

This project was developed by Gaurav Kasture in collaboration with Career247.

🚀 The Complexity: Solving for "Silent Churn"

Standard models often miss customers who don't complain but slowly disengage. This project solves for complexity using:

Friction Scoring: Aggregating network issues, late payments, and complaints into a single "pain index."

Charge Velocity: Measuring the rate at which a customer's monthly bill increases relative to their historical average (Detecting "Bill Shock").

Silent Risk Metric: A proprietary feature mapping high data usage against zero digital app engagement.

🛠️ Technical Stack & Architecture

We implemented a Stacked Ensemble Classifier to push accuracy and recall beyond baseline levels:

Base Learners (Level 0):

XGBoost: Configured as a "Careful Learner" with a low learning rate (0.01) to capture non-linear patterns.

Random Forest: Utilized for its robustness against outliers and feature importance mapping.

Meta-Model (Level 1):

Logistic Regression: Acts as a "Judge" to synthesize predictions from the base learners.

Threshold Tuning: Adjusted the classification threshold to 0.35 to prioritize Recall, ensuring we catch ~82% of potential churners.

📊 Results & Impact

Final Accuracy: ~74% (Significant improvement from 64% baseline).

Recall: ~82% (Optimized for business intervention).

ROC-AUC: 0.88 (High model confidence).

Estimated Business Impact: ~25% churn reduction in the high-value segment, preserving an estimated $2.4M USD in annual revenue.

📁 Repository Structure

telecom_churn_analysis.ipynb: The complete Google Colab notebook including EDA, Feature Engineering, and Modeling.

presentation.html: A professional slide deck summarizing the project for executive stakeholders.

telecom_churn.csv: The dataset used for analysis.

👨‍💻 Author

Gaurav Kasture 📧 gauravkasture@gmail.com

Partnered with Career247

Disclaimer: This project was conducted as part of a strategic data science initiative to improve customer lifecycle management.
