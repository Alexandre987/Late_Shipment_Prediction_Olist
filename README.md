# Late Shipment Prediction - Olist

Predicted late shipments for Brazilian retail company Olist, via Kaggle dataset: https://www.kaggle.com/olistbr/brazilian-ecommerce#olist_orders_dataset.csv

7.5% of Olist shipments are late. I only used data that is known *before* shipping in order to predict whether the shipment to the customer would be late, in order to improve their shipping estimates and reduce shipping times. My best model (Random Forest) performed with 53% recall, and 19% precision. The FBeta Score I used gave preference to recall, with the business case being that capturing all late shipments was more important than excluding shipments that arrived on time. It is better to send a warning email that a shipment might be late to too many people than too few, for instance.

Methods used:
- Logistic Regression
- K-Nearest Neighbors
- Random Forest
- SMOTE/ADASYN Upsampling (7.5% of shipments are late - imbalanced classes)

Feature importance of the Random Forest was used to determine the most predictive features of a late shipment, before it even reaches the trucks.
