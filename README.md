# credit-risk-model

“How does Basel II influence model choice?”

Basel II emphasizes accurate risk measurement, transparency, and accountability in credit decision-making. This means that models used by financial institutions must be interpretable, well-documented, and auditable. As a result, we prioritize models that allow clear explanation of how input features influence risk predictions. This ensures regulatory compliance, stakeholder trust, and easier validation compared to black-box models.

“Why do we need a proxy default variable?”


Since the dataset does not contain an explicit loan default label, creating a proxy target variable is necessary to approximate customer credit risk. We use behavioral indicators derived from transaction history, such as Recency, Frequency, and Monetary value, to identify disengaged customers who are more likely to default. However, this approach introduces business risk because the proxy may not perfectly reflect true default behavior, potentially leading to misclassification of customers.

“Simple vs complex models?”

Simple models such as Logistic Regression with Weight of Evidence (WoE) offer high interpretability and regulatory acceptance, making them suitable for financial institutions. However, they may lack predictive power. Complex models like Gradient Boosting can achieve higher accuracy but act as black boxes, making them harder to explain and validate. In a regulated environment, this creates a trade-off between performance and explainability, often requiring careful model selection and documentation.