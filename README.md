# 💊 pharmacy-demand-llm

AI-powered pharmacy demand forecasting and LLM-based clinical/business insight generation.

---

# Pharmacy Demand Forecasting & LLM Insights System

## Combining Time-Series Forecasting with Large Language Models for Operational Decision Support

This project presents an end-to-end AI system that combines traditional forecasting models with Large Language Models (LLMs) to generate interpretable pharmacy demand insights for inventory planning and staffing optimization.

The system integrates:

- Time-series forecasting
- Machine learning
- Feature engineering
- Large Language Models (LLMs)
- Reinforcement Learning from Human Feedback (RLHF)
- Natural language insight generation

The project explores how predictive AI systems can move beyond forecasting alone and support human decision-making through interpretable and actionable outputs.

---

# Project Objectives

This work investigates how AI systems can:

- Forecast pharmacy demand across multiple drug categories
- Capture seasonality and patient demand patterns
- Generate human-readable operational insights
- Support inventory and staffing decisions
- Improve interpretability of forecasting systems

The project combines predictive modelling with natural language reasoning to bridge the gap between machine-generated forecasts and human operational understanding.

---

# Key Features

## 📊 Time-Series Forecasting

The forecasting pipeline combines multiple modelling approaches:

### Prophet
- Trend and seasonality modelling
- Long-term demand forecasting
- Holiday and cyclic trend handling

### SARIMA
- Statistical time-series forecasting
- Seasonal autoregressive modelling
- Temporal pattern analysis

### XGBoost
- Feature-based machine learning forecasting
- Nonlinear demand pattern learning
- Structured feature optimization

---

## 🧩 Feature Engineering

The system includes extensive feature engineering techniques:

- Lag features (1-day, 7-day, 30-day)
- Rolling statistics (mean, standard deviation)
- Time-based features:
  - weekday,
  - month,
  - seasonal indicators
- Fourier transforms for cyclic demand patterns

These features improve temporal modelling and help capture patient behavior trends.

---

## 🤖 Large Language Model (LLM) Pipeline

The project integrates GPT-2 fine-tuning for natural language insight generation.

### Supervised Fine-Tuning (SFT)

The model was fine-tuned on custom instruction-response datasets designed for operational pharmacy analysis.

### RLHF Alignment

The project additionally explores:
- Reinforcement Learning from Human Feedback (RLHF)
- Preference pair generation
- Alignment optimization using DPO-based approaches

This enables the model to generate more interpretable and human-aligned responses.

---

# Output Capabilities

The system generates:

- 90-day pharmacy demand forecasts
- Trend analysis summaries
- Inventory planning insights
- Staffing optimization recommendations
- Human-readable forecasting explanations

---

# Example Use Case

## Input

> “Explain pharmacy sales trends during weekends.”

## Generated Insight

> Weekend demand reflects recurring patient pickup behavior and clinic scheduling patterns. Staffing allocation and inventory management should align with expected peak collection periods.

---

# Workflow

```plaintext
1. Data preprocessing and cleaning
2. Exploratory data analysis
3. Feature engineering
4. Forecasting model training and evaluation
5. LLM instruction dataset generation
6. GPT-2 supervised fine-tuning
7. RLHF preference optimization
8. Natural language insight generation
9. Forecast evaluation and interpretation
```

---

# Repository Structure

```plaintext
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
│   └── 08_rlhf_preference_tuning.ipynb
│
├── src/
├── docs/
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Technologies Used

## Forecasting and Machine Learning
- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Prophet
- SARIMA

## NLP and LLMs
- HuggingFace Transformers
- GPT-2
- TRL (DPOTrainer)
- RLHF-based alignment methods

## Visualization
- Matplotlib
- Plotly

---

# Experimental Focus

This project explores several broader AI themes:

- Interpretable forecasting systems
- Human-centered AI decision support
- Hybrid ML + LLM architectures
- AI-assisted operational planning
- Alignment and preference optimization
- Natural language generation for analytics systems

---

# Business and Operational Impact

Potential practical applications include:

- Improved pharmacy demand forecasting
- Inventory optimization
- Reduced stock shortages and overstocking
- Better staffing allocation
- Human-readable operational intelligence
- Improved interpretability of forecasting outputs

---

# Reliability and Limitations

Several important limitations remain:

## Forecast Uncertainty

Demand forecasting systems remain sensitive to:
- changing patient behavior,
- external events,
- seasonal anomalies,
- and unexpected demand spikes.

## LLM Reliability

Generated insights may occasionally:
- oversimplify patterns,
- hallucinate unsupported explanations,
- or fail to communicate uncertainty clearly.

## Real-World Deployment Challenges

Operational deployment would require:
- continuous monitoring,
- robust validation,
- human oversight,
- and real-time data integration.

This project represents an exploratory AI-assisted decision-support framework rather than a production healthcare system.

---

# Future Improvements

Potential future extensions include:

- FastAPI or Streamlit deployment
- Integration with real-time pharmacy systems
- Larger LLM architectures (LLaMA, Mistral)
- Uncertainty-aware forecasting
- Retrieval-Augmented Generation (RAG)
- Multi-agent forecasting pipelines
- Explainable AI for forecasting systems
- Anomaly detection for unusual demand spikes

---

# Documentation

📄 [View Full Project Report](docs/Pharmacy%20Demand%20Forecasting%20%26%20LLM-Based%20Decision%20Support%20System.pdf)

---

# Research Significance

This project reflects a broader research interest in:

- trustworthy AI systems,
- interpretable machine learning,
- AI-assisted decision support,
- and human-centered AI deployment.

The work explores how forecasting systems can evolve from predictive models into collaborative AI systems that generate operationally useful and interpretable insights.

---

# Author

## Venu Madhuri Yerramsetti

**Independent AI Researcher**  
**MSc Artificial Intelligence and Data Science — University of Hull**

### Research Interests

- AI-Assisted Decision Support
- Trustworthy AI
- Healthcare AI
- Explainable AI
- Time-Series Forecasting
- Human-AI Interaction
- Large Language Models
- Responsible AI

---

# Citation

```bibtex
@misc{yerramsetti2026pharmacyllm,
  author = {Venu Madhuri Yerramsetti},
  title = {Pharmacy Demand Forecasting and LLM-Based Decision Support System},
  year = {2026},
  note = {GitHub repository},
  url = {https://github.com/VenuYerramsetti/pharmacy-demand-llm}
}
```

---

# License

This repository is intended for academic and research purposes.
