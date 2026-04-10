# 🌌 Martian Atmospheric Forecasting using MEDA Data

This project presents a data-driven framework for modelling and forecasting near-surface atmospheric pressure on Mars using data from the Mars 2020 Perseverance rover (MEDA instrument suite).

The study combines classical machine learning and deep learning approaches to evaluate forecasting performance across multiple time horizons, with a strong emphasis on reproducibility, physical consistency, and robust evaluation.

---

## 🚀 Project Objectives

- Develop a structured and reproducible time-series dataset from NASA MEDA PDS data  
- Model Martian surface pressure using baseline, machine learning, and deep learning methods  
- Evaluate forecasting performance across multiple horizons (1h, 3h, 6h, 12h, 24h)  
- Analyse model behaviour under different atmospheric regimes  
- Incorporate uncertainty quantification and calibration  

---

## 📊 Models Used

| Model | Purpose |
|------|--------|
| Persistence | Baseline (temporal continuity) |
| Random Forest | Nonlinear pattern learning |
| LSTM | Sequential temporal modelling |
| Transformer | Long-range dependency modelling |

---

## 📈 Key Results

- **Random Forest** performs best at short horizons (1h–3h) due to strong autocorrelation  
- **Transformer** achieves the best long-term performance (24h), capturing diurnal periodicity  
- Forecast errors increase with horizon due to atmospheric variability  
- Relative error remains low (~1–2%), indicating high predictive accuracy  

---

## 📊 Evaluation Metrics

- MAE (Mean Absolute Error)  
- RMSE (Root Mean Squared Error)  
- R² (Coefficient of Determination)  
- MAPE (Mean Absolute Percentage Error)  
- CRPS (Continuous Ranked Probability Score)  

---

## 🧠 Key Insights

- Martian surface pressure exhibits strong temporal autocorrelation and diurnal periodicity  
- Classical models remain highly competitive in structured environmental data  
- Deep learning models provide advantages in capturing long-term dependencies  
- Proper time-series handling (chronological splits) is critical to avoid data leakage  

---

## 📂 Dataset

- Source: NASA Planetary Data System (PDS)  
- Instrument: MEDA (Mars Environmental Dynamics Analyzer)  
- Location: Jezero Crater (Mars)  
- Time Range: Sol 300 – Sol 419  

---

## ⚙️ Installation

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

Run notebooks in order:

1. Data Processing  
2. Feature Engineering  
3. Baseline Models  
4. LSTM Model  
5. Transformer Model  

---

## 📊 Results

Final results and model comparisons are available in the `/results` directory.

---

## 🔬 Reproducibility

- Chronological data splitting to avoid leakage  
- Fixed random seeds  
- Saved models and experiment outputs  

---

## 📌 Future Work

- Incorporate wind and additional atmospheric variables  
- Explore physics-informed neural networks  
- Extend to multi-location Martian datasets  

---

## 📄 Author

Tharindu Irushan  
MSc Data Science – Coventry University  

---

## 📜 License

This project is for academic and research purposes.
