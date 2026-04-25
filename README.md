# 💊 Pharmacy Demand Forecasting & LLM Insights System

An end-to-end AI system combining time-series forecasting and Large Language Models (LLMs) to generate actionable pharmacy insights for inventory planning and staffing optimization.

---

## 🚀 Project Overview

This project integrates traditional machine learning with modern NLP techniques to:

- Forecast pharmacy demand across multiple drug categories
- Capture temporal trends, seasonality, and patient behavior patterns
- Generate human-readable insights using fine-tuned LLMs
- Support operational decision-making (inventory & staffing)

---

## 🧠 Key Features

### 📊 Time Series Forecasting
- Prophet (trend + seasonality modeling)
- SARIMA (statistical forecasting)
- XGBoost (feature-based ML model)

### 🧩 Feature Engineering
- Lag features (1, 7, 30 days)
- Rolling statistics (mean, std)
- Time-based features (weekday, month, seasonality)
- Fourier transforms for cyclic patterns

### 🤖 LLM Pipeline
- GPT-2 fine-tuned using:
  - Supervised Fine-Tuning (SFT)
  - Reinforcement Learning with Human Feedback (RLHF)
- Custom instruction dataset generation
- Preference pair creation for alignment

### 📈 Output Capabilities
- Demand forecasts (90-day horizon)
- Business insights generation
- Staffing & inventory recommendations

---

## 🏗️ Project Structure
pharmacy-demand-llm/
│
├── notebooks/
│   ├── 01_data_preparation.ipynb
│   ├── 02_eda_visualizations.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_ml_models_forecasting.ipynb
│   ├── 05_model_comparison.ipynb
│   ├── 06_forecasting_models_prophet_sarima_xgboost_90_day_horizon.ipynb
│   ├── 07_llm_pipeline_SFT_FineTuning_with_GPT2.ipynb
│   ├── 08_rlhf_preference_tuning.ipynb
│
├── src/
├── README.md
├── requirements.txt

---

## ⚙️ Tech Stack

- Python (pandas, numpy, sklearn)
- Time Series: Prophet, SARIMA, XGBoost
- NLP: HuggingFace Transformers (GPT-2)
- RLHF: TRL (DPOTrainer)
- Visualization: Matplotlib, Plotly

---

## 🔍 Workflow

1. Data preprocessing & cleaning  
2. Exploratory data analysis  
3. Feature engineering  
4. Forecasting model training & evaluation  
5. LLM dataset generation (instructions + responses)  
6. SFT fine-tuning of GPT-2  
7. RLHF-based alignment using preference optimization  
8. Insight generation & evaluation  

---

## 📊 Example Use Case

Input:
> "Explain pharmacy sales trends during weekends"

Output:
> Weekend demand reflects predictable patient pickup patterns and clinic schedules. Staffing and inventory should align with peak collection times.

---

## 🎯 Business Impact

- Improves demand forecasting accuracy  
- Enables data-driven staffing decisions  
- Reduces stockouts and overstocking  
- Enhances interpretability of ML outputs  

---

## 🚀 Future Improvements

- Deploy as API (FastAPI / Streamlit)
- Upgrade to larger LLMs (LLaMA, Mistral)
- Integrate real-time pharmacy data
- Add anomaly detection for unusual demand spikes

---

## 📄 Documentation

👉 [View Full Project Report](docs/Pharmacy%20Demand%20Forecasting%20%26%20LLM-Based%20Decision%20Support%20System.pdf)

---

## 👩‍💻 Author

**Venu Madhuri Yerramsetti**  
Data Scientist | ML Engineer | MSc AI & Data Science (UK)

- GitHub: https://github.com/VenuYerramsetti  
- LinkedIn: https://www.linkedin.com/in/venu-madhuri-yerramsetti-349057aa  

---

## ⭐ If you found this useful, consider starring the repo!
