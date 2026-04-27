# British-Airways-passenger-data-Analytics
Built a British Airways booking prediction model to forecast customer purchases using booking data. Applied data cleaning, feature engineering, imbalance handling, and trained a Random Forest classifier. Evaluated with cross-validation and ROC-AUC, then interpreted feature importance for actionable marketing insights.

British Airways Booking Prediction
A machine learning project focused on predicting whether a customer will complete a booking using British Airways customer booking data.

Overview
This project explores customer booking behavior and builds a predictive model to identify which customers are most likely to complete a booking. The goal is to support proactive marketing decisions by helping the business target high-intent customers before travel.

Dataset
The dataset contains customer booking records with features such as:

Number of passengers

Purchase lead time

Length of stay

Flight hour and duration

Route and booking origin

Sales channel and trip type

Ancillary preferences such as extra baggage, preferred seat, and in-flight meals

Approach
The workflow included:

Data cleaning and initial exploration

Feature engineering, including trip complexity, premium score, booking timing bands, and cyclical flight-hour features

Encoding categorical variables

Handling class imbalance with SMOTE

Training a Random Forest classifier

Evaluating performance using cross-validation and ROC-AUC

Interpreting feature importance for business recommendations

Key Results
The model delivered strong predictive performance:

Metric	Value	Interpretation
AUC-ROC	0.87	Excellent discrimination between classes
Cross-validation score	0.86 ± 0.03	Stable performance across folds
Recall (bookers)	0.82	Captures most actual bookers
Precision (bookers)	0.52	Useful for proactive targeting
F1-score	0.63	Good balance between recall and precision
Top Predictive Features
The most important features were:

Purchase lead time

Route

Trip complexity

Length of stay

Premium score

These results suggest that early planners, specific routes, more complex trips, and customers selecting ancillaries are more likely to complete a booking.

Business Insights
Customers booking well in advance show stronger purchase intent.

Route selection has a major influence on booking completion probability.

Customers choosing extras such as baggage, meals, or preferred seats are higher-intent segments.

The model can support targeted campaigns, better customer segmentation, and more efficient marketing spend.

Tech Stack
Python

pandas

NumPy

scikit-learn

imbalanced-learn

Matplotlib

Seaborn

Outcome
This project demonstrates how machine learning can turn booking data into actionable commercial insight. The final model is interpretable, performs well on imbalanced data, and provides clear business value for customer acquisition strategy.
