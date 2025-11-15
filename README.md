☀️ Predicting Eskom’s Solar PV Installation and Electricity Production in South Africa
A reproducible analysis and forecasting pipeline for South Africa’s solar PV generation (2021–2025) with projections to 2030, built in Python 🐍 and designed for transparent, examiner-ready outputs 📊.

📖 Overview

🎯 Goal: Quantify historical solar PV generation and forecast 2026–2030 outputs.

📂 Data: Eskom, CSIR, DMRE datasets (2021–2025).

🧮 Methods: Descriptive stats, correlation analysis, Prophet time-series, Linear Regression, Random Forest.

🖼️ Outputs: Figures in Chapter4_Figures/ + CSV tables in outputs/tables/.

📂 Repository Structure text.

├── data/                     # 📊 Input datasets

├── notebooks/                # 📓 Exploratory notebooks

├── src/                      # ⚙️ Core scripts

├── outputs/                  # 📈 Figures + tables

├── environment.yml           # 🐍 Conda environment

├── requirements.txt          # 📦 Pip dependencies

└── README.md                 # 📘 This file

⚙️ Environment Setup
🐍 Python 3.10–3.13

Install with conda:
bash
conda env create -f environment.yml
conda activate eskom-pv
Or with pip:

bash
python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
🚀 Quick Start
1️⃣ Place cleaned dataset in data/eskom_pv_2021_2025.csv. 2️⃣ Run the pipeline:

bash
python src/preprocess.py

python src/analysis_descriptive.py

python src/analysis_trends.py

python src/model_prophet.py

python src/model_ml.py

📊 Outputs → outputs/Chapter4_Figures/ 📑 Tables → outputs/tables/

📈 Key Figures

📉 Line plot: PV generation (2021–2025)

📦 Boxplots: Annual & monthly PV output

🔮 Forecasts: Predicted vs. actual PV (2026–2030)

🌐 Correlation heatmap: irradiance, capacity, UCLF


📝 Results Summary

✅ Cleaned dataset: ~35,546 valid hourly observations

⚡ Historical generation (2021–2025): ≈ 20.82 TWh

🔮 Forecast by 2030: ~16.2–16.4 TWh annually

🤖 Model performance: RF 

𝑅2≈0.92, LR 𝑅2≈0.85

📜 Citation

Qadi, Y. (2025). Predicting Eskom’s Solar PV Installation and Electricity Production in South Africa.

📄 License

MIT or CC BY 4.0 recommended — update LICENSE accordingly.

🙌 Acknowledgements

👩‍🏫 Supervisor: XXXXXX

🔌 Data: Eskom, CSIR, DMRE

🐍 Tools: Python ecosystem (pandas, scikit-learn, prophet, matplotlib)

📬 Contact

👩 Author: Yolisa Qadi (ST10472252)

📧 Email: yolisaqadi12@gmail.com

🌍 Location:South Africa
