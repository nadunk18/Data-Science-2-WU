
# 🎵 Fairness-Aware Music Recommendation with RecBole and AIF360

This project explores genre popularity bias in music recommendation systems using the RecBole library and fairness evaluation via AIF360. The pipeline includes data preprocessing, model training, genre skew analysis, and fairness evaluation using simulated gender as a protected attribute.

---

## 📌 Project Overview

The goal is to understand and mitigate genre-based popularity bias in music recommendations and evaluate fairness across user demographics using AIF360. Specifically, we:

- Analyze genre distribution and skew in the dataset
- Train a recommendation model using RecBole
- Simulate user gender to test for demographic bias
- Apply fairness metrics from AIF360

---

## 🛠️ Tech Stack

- Python 3.10+
- [RecBole](https://recbole.io)
- [AIF360](https://aif360.readthedocs.io/)
- NumPy, pandas, matplotlib
- scikit-learn
- Jupyter / Kaggle Notebook

---

## 📁 Folder Structure & File Paths

> To ensure reproducibility and avoid path errors, follow this suggested structure and use **relative paths** in code.

```
.
├── data/                   # Raw and preprocessed datasets
│   ├── lastfm_ratings.csv
│   └── user_metadata.csv            # Includes gender, age, location
├── configs/                # RecBole YAML config files
│   └── lastfm.yaml
├── notebooks/             
│   └── Music_DS_Final.ipynb
├── outputs/                # Logs, trained models, and results
│   ├── log/
│   └── recbole_output/
├── fairness/               # Fairness metrics and visualizations
│   └── metrics_summary.csv
├── README.md
└── requirements.txt
```

### 🔄 Path Recommendations in Code

- Use **relative paths** (e.g., `./data/lastfm_ratings.csv`, not absolute system paths)
- Ensure folders like `fairness/`, `outputs/`, and `configs/` are created before writing output files

---

## 📊 Dataset

Two datasets are used in this project:

1. **lastfm_ratings.csv** – user-item interaction data (implicit feedback)
2. **user_metadata.csv** – contains user-level metadata (e.g., simulated gender, age, location)

Both datasets are preprocessed for compatibility with RecBole and fairness analysis.

---

## 🚀 How to Run

1. **Clone this repo**

```bash
git clone https://github.com/your-username/music-recbole-fairness.git
cd music-recbole-fairness
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Launch notebook**

Run `notebooks/Music_DS_Final.ipynb` in Jupyter or your IDE.

---

## ✅ Results

- Identified significant genre popularity imbalance
- Trained RecBole model and generated top-N recommendations
- Evaluated fairness using AIF360 with simulated gender
- Highlighted demographic differences in recommendation exposure

---

## 📄 License

This project is licensed under the MIT License.

---

## 🤝 Acknowledgements

- [RecBole](https://github.com/RUCAIBox/RecBole)
- [AIF360](https://github.com/Trusted-AI/AIF360)
- [Last.FM](https://www.last.fm)
