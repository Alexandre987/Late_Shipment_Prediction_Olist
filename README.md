# project_03

Predicted late shipments for Brazilian retail company Olist, via Kaggle dataset: https://www.kaggle.com/olistbr/brazilian-ecommerce#olist_orders_dataset.csv

7.5% of Olist shipments are late. I only used data that is known pre-shipping in order to predict whether the shipment to the customer would be late, in order to improve their shipping estimates and reduce shipping times. Best model (Random Forest) performed with 53% recall, and 19% precision. FBeta Score used gave preference to recall, with the business case that longer  shipping time estimates primarily require higher recall, rather than higher precision.

Methods used:
- Logistic Regression
- K-Nearest Neighbors
- Random Forest
- SMOTE/ADASYN Upsampling (7.5% of shipments are late - imbalanced classes)
