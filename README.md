## 💳 FinShield AI Assistant

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-Chatbot-FF4B4B?logo=streamlit&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn%20%7C%20LightGBM-F7931E?logo=scikitlearn&logoColor=white)
![XAI](https://img.shields.io/badge/Explainable%20AI-SHAP-8A2BE2)
![NLP](https://img.shields.io/badge/NLP-TF--IDF%20Sentiment-6A1B9A)
![Time Series](https://img.shields.io/badge/Forecasting-ARIMA-11557C)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Classification](https://img.shields.io/badge/Task-Classification-success)
![Clustering](https://img.shields.io/badge/Task-Segmentation-success)
![Anomaly Detection](https://img.shields.io/badge/Task-Fraud%20Detection-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

An end-to-end financial intelligence platform that turns raw customer, credit, market, economic and news data into a unified **FinShield Score (0–1000)** is paired with SQL based analytics, explainable credit-risk classification (SHAP), fraud/anomaly detection, market forecasting, NLP sentiment analysis, a decision-support recommendation engine and an interactive AI chatbot for real-time customer risk lookup.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Analysis Phases](#analysis-phases)
- [Key Insights](#key-insights)
- [Strategic Recommendations](#strategic-recommendations)
- [Tools & Technologies](#tools--technologies)
- [How to Run](#how-to-run)
- [How to Run the Chatbot](#how-to-run-the-chatbot)
- [Summary Table](#summary-table)
- [License](#license)
- [Author](#author)

---

## Project Introduction

In today's rapidly evolving financial landscape, individuals, financial institutions, and investors face increasing challenges in accurately assessing financial risk and making informed investment decisions. Traditional risk assessment methods often rely on manual analysis, historical data interpretation and expert judgment of approaches that are slow, prone to bias, and unable to adapt to dynamic market conditions. Many ML-based financial systems also operate as "black boxes," offering predictions without explaining the reasoning behind them.

**FinShield AI** is an intelligent, data-driven financial analytics platform designed to close that gap by combining Machine Learning with Explainable AI. The platform ingests customer profiles, credit history, transaction behavior, market data, macroeconomic indicators, and financial news to predict credit risk, detect fraud, forecast market movement, gauge sentiment and produce a single, transparent financial-health score as per customer surfaced through an interactive Power BI-ready dataset and a conversational chatbot.

The project is delivered across three notebooks that form one continuous pipeline:

1. **Part 1 : Data Foundation & Engineering** (`Data_Engineering.ipynb`)
2. **Part 2 : Machine Learning Engine** (`Risk_Intelligence.ipynb`)
3. **Part 3 : Intelligence, Scoring & Explainability** (`FinShield_Engine.ipynb`)

---

## 📖 Problem Statement

Develop an end-to-end AI-powered financial intelligence platform that predicts customer credit risk, evaluates financial health, detects anomalous behavior, segments customers based on financial profiles, and provides personalized, explainable recommendations of combining machine learning, explainable AI, business intelligence and an AI chatbot to support transparent, data-driven decision-making for financial institutions.

Using the **Home Credit Default Risk** dataset as the customer behavioral backbone, the system analyzes demographics, employment history, income, credit information and loan characteristics to estimate default probability, generate interpretable risk scores and recommend appropriate financial actions improving loan approval decisions, reducing credit risk and supporting financial advisors through an interactive assistant.

---

## 🎯 Objectives of the Study

**Primary Objective:**
To develop an intelligent financial risk assessment and investment decision-support platform that leverages Machine Learning (ML) and Explainable AI (XAI) to provide accurate, transparent, and data-driven financial insights.

**Specific Objectives:**
- To collect, clean and preprocess customer, credit, market, economic and news data for predictive modeling.
- To design a relational (SQL) data foundation for structured storage and querying.
- To identify the key financial indicators that influence credit risk and financial health.
- To develop and compare multiple ML models (Logistic Regression, Random Forest) for risk-tier classification.
- To detect anomalous/fraudulent financial behavior using Isolation Forest.
- To forecast market movement per company using ARIMA time-series models.
- To score financial news sentiment using TF-IDF and classify its market impact.
- To engineer a composite **FinShield Score (0–1000)** blending credit, market, economic and sentiment risk.
- To integrate Explainable AI (SHAP) for transparent, individual-level risk explanations.
- To build an AI Recommendation Engine that converts risk scores into concrete monitoring actions.
- To develop an interactive **AI chatbot** that lets users query a customer's FinShield profile in natural language.

---

## 📚 Scope of the Study

- **Data Engineering** is building customer profile, transaction, and credit-history tables from the Home Credit dataset; generating synthetic market, economic, and news datasets.
- **SQL Database Design** a storage of raw, cleaned, and model-enriched tables.
- **Exploratory Data Analysis (EDA)** makes demographic distributions, correlation heatmaps, credit-risk relationships.
- **Feature Engineering**do debt-to-income ratios, credit utilization, behavioral risk ratios.
- **Machine Learning**makes multi-class credit-risk classification (Low/Medium/High/Critical), Isolation Forest fraud detection, K-means-style customer segmentation.
- **Time Series & NLP** is ARIMA market forecasting, TF-IDF financial-news sentiment scoring.
- **Explainable AI** gives global and individual SHAP-based risk explanations.
- **Decision Support** give rule-based AI Recommendation Engine and alert-level triage.
- **Conversational AI** a lightweight chatbot interface for natural-language, real-time customer risk lookup.

**Out of scope:** real-time trading, high-frequency trading algorithms, cryptocurrency prediction, automated portfolio execution and payment-gateway integration.

---

## 📊 Dataset

**Primary source:** Home Credit Default Risk dataset (application-level customer data), sampled to **60,000 customers**.

**Derived / synthetic tables built in Part 1:**
| Table | Description |
|---|---|
| `customer_profile` | Demographics - age, gender, occupation, education, city tier, family status |
| `financial_transactions` | Monthly income/expense, savings, investments, loan amount, EMI, transaction count |
| `credit_history` | Credit score, previous loans, late payments, credit-card count, credit utilization |
| `market_data` | Daily OHLC-style price series for 10 synthetic companies (ALPHA–JOVIAN), 2024–2025 |
| `economic_indicators` | Monthly GDP growth, inflation, interest rate, unemployment |
| `news_sentiment` | Synthetic financial headlines labeled Positive / Negative / Neutral per company |

---

## 🗂️ Project Structure

```
FinShield-AI-Assistant/
├── .devcontainer/
│   └── devcontainer.json
│
├── Chatbot Visuals/
│   ├── App-Running-Working.mp4
│   ├── Customer Table.png
│   ├── Executive Dashboard.png
│   ├── Front Interface.png
│   ├── Front Interface 2.png
│   ├── Image & Video Analysis.png
│   ├── LLM Provider.png
│   ├── Predefined Questions.png
│   └── System Health.png
│
├── Dashboard/
│   ├── Customer Table.png
│   └── Executive Dashboard.png
│
├── Data/
│   ├── Processed/
│   │   ├── credit_history_clean.xls
│   │   ├── customer_profile_clean.xls
│   │   ├── economic_indicators_clean.xls
│   │   ├── financial_transactions_clean.xls
│   │   ├── market_data_clean.xls
│   │   └── news_sentiment_clean.xls
│   └── Raw/
│       ├── credit_history.xls
│       ├── customer_profile.xls
│       ├── economic_indicators.xls
│       ├── financial_transactions.xls
│       ├── market_data.xls
│       └── news_sentiment.xls
│
├── Documentation/
│   ├── FinShield AI Assistant Report.pdf
│   └── FinShield-AI-Assistant.pptx
│
├── FinShield Chatbot/
│   ├── Outputs/
│   │   ├── company_sentiment_impact.csv
│   │   ├── finshield_scores.csv
│   │   ├── fraud_scores.csv
│   │   ├── market_forecasts.csv
│   │   └── risk_monitoring_decisions.csv
│   ├── .env.example
│   ├── app.py
│   ├── requirements.txt
│   └── secrets.toml
│
├── Models/
│   ├── fraud_isolation_forest.pkl
│   ├── risk_classifier_logreg.pkl
│   ├── risk_classifier_rf.zip
│   ├── risk_scaler.pkl
│   ├── sentiment_classifier.pkl
│   └── sentiment_vectorizer.pkl
│
├── Notebook/
│   ├── Data Engineering.ipynb
│   ├── FinShield Engine.ipynb
│   └── Risk Intelligence.ipynb
│
├── SQL/
│   └── FinShield_DB.sqlite
│
├── Visuals/
│   ├── Credit Score Distribution by Loan Status.png
│   ├── Customer Age Distribution.png
│   ├── Financial & Credit Risk Correlation Matrix.png
│   ├── Loan Default Distribution.png
│   ├── Macroeconomics Indicators Trend.png
│   ├── Monthly Income vs Expense.png
│   └── Top 15 Features by SHAP Importance.png
│
├── LICENSE
└── README.md
```

---

## 🔍 Analysis Phases

### Part 1 : Data Foundation & Engineering
- **Phase 1:** Data Acquisition & Business Understanding
- **Phase 2:** Data Cleaning + Handling Missing Values & Outliers
- **Phase 3:** SQL Database Design & Loading
- **Phase 4:** Exploratory Data Analysis (age, defaults, income vs. expenses, credit score vs. default, correlation heatmap, market/economic trends)

### Part 2 : Machine Learning Engine
- **Phase 5:** Risk Classification (Low / Medium / High / Critical), Logistic Regression & Random Forest
- **Phase 6:** Fraud / Anomaly Detection & Isolation Forest on behavioral ratios
- **Phase 7:** Market Forecasting with ARIMA per company
- **Phase 8:** NLP Financial Sentiment using TF-IDF + classifier, company-level impact scoring

### Part 3 : Intelligence, Scoring & Explainability
- **Phase 9:** The FinShield Score (0–1000) that blending credit, market, economic & sentiment risk into a Financial Health tier
- **Phase 10:** Explainable AI (SHAP) that give global feature importance & individual customer explanations
- **Phase 11:** Risk Monitoring & Segmentation with alert levels (Normal/Watch/Warning/Critical) & behavioral segments
- **Phase 12:** AI Recommendation Engine (Decision Center) rule-based recommended actions per customer
- **Phase 13:** Business Insight
- **Phase 14:** Strategic Recommendations
- **Phase 15:** Executive Summary, Future Scope & Conclusion

---

## 💡 Key Insights

1. **Credit risk is concentrated in Medium/High segments**  28,062 customers Medium-risk and 24,642 High-risk, vs. 6,133 Low and 1,163 Critical, out of 60,000.
2. **Credit score is the strongest predictor of risk**  ~66.5% of Random Forest feature importance, followed by late payments (~11.5%) and credit utilization (~7.1%).
3. **Late payments are an early-warning signal** the second most important feature, and ~23.7% of SHAP importance in high-risk explanations.
4. **A meaningful default population exists**  4,817 of 60,000 customers (8.03%) have recorded loan defaults, with an average credit score of 516.9 vs. 585.4 for non-defaulters.
5. **Fraud monitoring adds an independent risk signal**  Isolation Forest flagged 1,200 of 60,000 customers (2.0%) as behaviorally anomalous.
6. **Market and sentiment context sharpen the picture**  ARIMA forecasts and TF-IDF news-sentiment impact scores (e.g., INDUS +0.182, GRANITE −0.003) feed directly into the FinShield Score's market/sentiment components.
7. **SHAP delivers transparent, individual-level explanations**, letting risk teams see exactly why a customer was scored the way they were — beyond a single classification label.

---

## 🧭 Strategic Recommendations

1. **Prioritize proactive intervention** for High and Critical-risk customers, credit restructuring, repayment planning, financial counselling.
2. **Build an early-warning system** around credit score and late-payment trends, triggering automatic risk-score refreshes on deterioration.
3. **Combine fraud alerts with credit-risk scores** customers flagged on both dimensions should receive top priority in the FinShield Priority Alert workflow.
4. **Introduce differentiated lending policies** by risk segment instead of applying uniform credit terms.
5. **Manage investment exposure using market-risk and sentiment signals** alongside credit fundamentals.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Programming |
| Pandas / NumPy | Data analysis & numerical computing |
| Matplotlib / Seaborn | EDA visualization |
| SQLite | Relational database & SQL analytics |
| Scikit-learn | Classification, anomaly detection, scaling, TF-IDF |
| LightGBM | Gradient-boosted modeling support |
| Statsmodels (ARIMA) | Market time-series forecasting |
| SHAP | Explainable AI (global & local feature importance) |
| Streamlit | Interactive AI chatbot interface |
| Jupyter Notebook | Development environment |

---

## ▶️ How to Run

```bash
pip install pandas numpy scikit-learn lightgbm statsmodels shap joblib matplotlib seaborn streamlit --break-system-packages
jupyter notebook
```

1. Place the Home Credit `application_train.csv` file where **Part 1** expects it, and update that file path in `Data_Engineering.ipynb`.
2. Run `Data_Engineering.ipynb` (Part 1) first, start to finish & builds `Data/raw/`, `Data/processed/`, and the SQL tables that later notebooks depend on.
3. Run `Risk_Intelligence.ipynb` (Part 2) next then trains and saves the risk classifier, fraud model, ARIMA forecasts, and sentiment model to `Models/` and `outputs/`.
4. Run `FinShield_Engine.ipynb` (Part 3) last then computes the FinShield Score, SHAP explanations, alert levels, and recommended actions, saving `outputs/finshield_scores.csv` and `outputs/risk_monitoring_decisions.csv`.
5. (Optional) Load the `outputs/` CSVs into Power BI for a dashboard view.

---

## 🤖 How to Run the Chatbot

`chatbot_app.py` is a lightweight **Streamlit** chatbot that sits on top of the pipeline's final outputs. It lets a user type a customer ID (or ask a natural-language question) and get back that customer's FinShield Score, Financial Health tier, alert level and recommended actions in a conversational format.

**Prerequisite:** Parts 1–3 must have already been run at least once, so that `outputs/finshield_scores.csv` and `outputs/risk_monitoring_decisions.csv` exist.

```bash
pip install streamlit pandas --break-system-packages
streamlit run app.py
```

1. This launches the chatbot in your browser at `http://localhost:8501`.
2. Type a customer ID (e.g. `C10004`) or ask a question like *"What's the risk status of C10004?"*.
3. The chatbot looks up the customer in `outputs/risk_monitoring_decisions.csv` and `outputs/finshield_scores.csv` and replies with:
   - FinShield Score (0–1000) and Financial Health tier
   - Alert level (Normal / Watch / Warning / Critical)
   - Fraud-flag status
   - Recommended actions from the AI Recommendation Engine
4. To stop the chatbot, close the browser tab and press `Ctrl+C` in the terminal.

> **Note:** This chatbot is intentionally rule-based and reads directly from the saved model outputs rather than calling an external LLM, so it runs fully offline with no API key required — suitable for demo/submission purposes. See *Future Scope* for plans to extend it into a full generative, conversational financial assistant.

---

## Summary Table

| Model | Accuracy | F1 (macro) | ROC-AUC |
|---|---|---|---|
| Logistic Regression | 73.4% | 0.648 | 0.93 |
| Random Forest | 73.4% | 0.648 | 0.93 |

| Metric | Value |
|---|---|
| Total customers analyzed | 60,000 |
| Loan-default customers | 4,817 (8.03%) |
| Fraud/anomalies flagged | 1,200 / 60,000 (2.0%) |
| Risk-tier distribution | Low: 6,133 · Medium: 28,062 · High: 24,642 · Critical: 1,163 |
| Companies covered (market/sentiment) | 10 |
| News-sentiment classifier accuracy | 100% (synthetic headline set) |

---

## 📄 License

Copyright © 2026 Uday Sahu

All Rights Reserved.

This project and all associated files, including but not limited to source code, notebooks, reports, dashboards, visualizations, documentation and datasets, are the exclusive intellectual property of Uday Sahu.

No part of this project may be copied, reproduced, modified, distributed, published, sublicensed, displayed, transmitted or sold in any form or by any means without the prior written permission of the copyright holder.

Permission is granted only to view this project for personal, educational or portfolio evaluation purposes. Commercial use, redistribution and creation of derivative works are strictly prohibited.

Unauthorized use, reproduction or distribution of this project may result in legal action under applicable copyright laws.

For permissions or licensing inquiries, please contact the copyright holder directly.

---

## 🙋 Author

**Uday Sahu**

**Data Analyst | Python | SQL | Power BI | Data Visualization | Business Analytics**

Passionate about transforming raw data into meaningful business insights through analytics, visualization and automation.

---

⭐ **If you found this project helpful, consider giving it a Star!**
