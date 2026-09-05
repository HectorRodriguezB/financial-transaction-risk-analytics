# Project Charter

## Project Title

Financial Transaction Risk Analytics

## Project Status

Planning

## 1. Project Overview

This project aims to build an end-to-end analytics solution for financial transaction risk and fraud analysis.

The first stage of the project will focus on descriptive and diagnostic analytics using SQL, Python, PostgreSQL, and Power BI. The project will later evolve into a predictive machine learning solution for fraud detection.

The project is designed to simulate a real-world Risk Analytics environment in which large volumes of financial transactions must be monitored, analyzed, and translated into actionable information for decision-making.

---

## 2. Business Context

A digital financial services company processes a large volume of transactions every day.

Because manually reviewing every transaction is not feasible, the Risk Operations team requires analytical tools to monitor transaction activity, quantify fraud exposure, identify suspicious behavioral patterns, and evaluate the effectiveness of existing fraud detection mechanisms.

The analytical solution should help the organization better understand where fraud occurs, how it behaves, and which transactions or accounts may require additional investigation.

---

## 3. Primary Stakeholder

### Risk Operations Manager

The primary stakeholder needs visibility into:

- Transaction volume and monetary value.
- Fraud frequency and financial exposure.
- Fraud patterns by transaction type and time.
- Potentially suspicious accounts or transaction behaviors.
- Performance of existing fraud alerts.
- Operational indicators that can support investigation priorities.

### Secondary Stakeholder

The Fraud Analytics / Data Science team may use the analytical findings and engineered features as inputs for future predictive models.

---

## 4. Main Business Objective

Develop a financial transaction risk analytics solution that helps identify, quantify, and understand fraud patterns using transactional data.

The solution should provide useful indicators and analytical tools to support Risk Operations decision-making.

A later phase of the project will extend the solution by developing machine learning models capable of estimating the probability that a transaction is fraudulent.

---

## 5. Business Questions

### Transaction Activity

1. How many transactions are processed?
2. What is the total monetary value processed?
3. How does transaction activity change over time?
4. Which transaction types represent the largest share of activity?
5. How do transaction amounts differ across transaction types?

### Fraud and Risk

6. What percentage of transactions are fraudulent?
7. What percentage of transaction value is associated with fraud?
8. Which transaction types present the highest fraud risk?
9. When is fraudulent activity most concentrated?
10. How do fraudulent transaction amounts differ from legitimate transactions?

### Account Behavior

11. Which origin accounts show unusually high transaction activity?
12. Are there destination accounts receiving unusually large or frequent transactions?
13. Are there behavioral patterns associated with fraudulent transactions?
14. Are abnormal balance changes associated with fraud?

### Existing Fraud Detection

15. How effective is the existing fraud flagging mechanism?
16. How many fraudulent transactions are successfully flagged?
17. How many fraudulent transactions remain undetected?
18. Does the current flagging mechanism generate false positives?

---

## 6. Initial Key Performance Indicators

### Operational KPIs

- Total Transactions
- Total Transaction Value
- Average Transaction Amount
- Median Transaction Amount
- Active Origin Accounts
- Active Destination Accounts

### Risk KPIs

- Fraudulent Transactions
- Fraud Rate
- Fraudulent Transaction Value
- Fraud Value Rate
- Average Fraud Amount

### Detection KPIs

- Flagged Transactions
- Detection Rate
- False Positive Rate
- False Negative Rate

Additional KPIs may be created as the analysis develops.

---

## 7. Dataset

The project will initially use the PaySim synthetic financial transaction dataset.

PaySim simulates financial transaction activity and includes information related to:

- Transaction type.
- Transaction amount.
- Origin account.
- Destination account.
- Account balances.
- Fraud labels.
- Existing fraud flags.
- Transaction time.

The dataset is synthetic and will be treated transparently as such throughout the project documentation.

The final dataset structure and data dictionary will be documented after the raw data has been acquired and inspected.

---

## 8. Initial Technology Stack

The planned technology stack includes:

- Python
- SQL
- PostgreSQL
- Power BI
- Git
- GitHub
- Visual Studio Code

Additional tools will only be introduced when they solve a specific project requirement.

---

## 9. Project Scope

### Phase 1 — Data Analytics and Business Intelligence

The first phase will include:

- Data acquisition.
- Data validation.
- Data cleaning and transformation.
- PostgreSQL database design.
- Data ingestion.
- SQL analysis.
- Exploratory data analysis with Python.
- Risk and fraud KPI development.
- Power BI dashboard development.
- Business findings and recommendations.

### Phase 2 — Data Science

The second phase will include:

- Feature engineering.
- Train/test strategy.
- Baseline model.
- Classification models.
- Class imbalance analysis.
- Model evaluation.
- Threshold selection.
- Model interpretability.
- Business-oriented error analysis.

---

## 10. Initial Deliverables

The project is expected to produce:

- Reproducible data ingestion process.
- PostgreSQL analytical database.
- Documented SQL analysis.
- Python exploratory analysis.
- Risk and fraud KPIs.
- Power BI dashboard.
- Business insights and conclusions.
- Machine learning fraud detection pipeline.
- Technical documentation.
- Professional GitHub repository.

---

## 11. Success Criteria

### Analytics Phase

The analytics phase will be considered complete when:

1. Raw data can be processed and loaded reproducibly.
2. Data quality and consistency have been validated.
3. Core business questions can be answered using SQL and Python.
4. Relevant risk KPIs have been defined and calculated.
5. A Power BI dashboard communicates the most important findings.
6. Conclusions are clearly connected to business decisions.
7. An external reviewer can understand the project structure and methodology from the repository documentation.

### Data Science Phase

The predictive phase will be considered complete when:

1. A reproducible modeling dataset has been created.
2. Data leakage has been appropriately controlled.
3. A meaningful baseline has been established.
4. Multiple justified modeling approaches have been evaluated.
5. Model performance is assessed using metrics appropriate for highly imbalanced classification.
6. The trade-off between false positives and false negatives is analyzed.
7. A final model and decision threshold can be justified from both technical and business perspectives.

---

## 12. Out of Scope

The following are not part of the initial scope:

- Real-time streaming infrastructure.
- Cloud infrastructure requiring paid enterprise services.
- Kubernetes.
- Deep learning without a demonstrated need.
- Production banking deployment.
- Real customer financial data.
- Technologies added only for portfolio visibility without a clear technical purpose.

---

## 13. Documentation Strategy

Project documentation will evolve together with the implementation.

Documents will be created only when the corresponding project stage requires them.

The initial documentation consists of:

- `README.md` — public project overview.
- `docs/project_charter.md` — project objectives, scope, stakeholders, questions, and success criteria.

Future documentation may include:

- Data dictionary.
- Database design documentation.
- Methodology documentation.
- Model evaluation documentation.