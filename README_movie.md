
# 🎬 Fairness-Aware Movie Recommendation using RecBole and AIF360

This project investigates fairness and popularity bias in movie recommendation systems. It uses RecBole for training collaborative filtering models and IBM's AIF360 for analyzing how recommendations differ across demographic attributes, with a focus on simulated gender.

---

## 📌 Project Overview

Our primary objectives:

- Detect popularity bias in movie genres
- Evaluate how user demographics (simulated gender) affect recommendation outcomes
- Use fairness metrics to identify imbalances in exposure

This project processes movie interaction datasets and metadata, trains RecBole models, and assesses fairness using AIF360.

---

## 🛠️ Tech Stack

- Python 3.10+
- [RecBole](https://recbole.io)
- [AIF360](https://aif360.readthedocs.io/)
- pandas, NumPy, matplotlib
- scikit-learn
- Jupyter / Kaggle Notebook

---

## 📁 Folder Structure & File Paths

```bash
.
├── data/
│   ├── movie_ratings.csv           # User-item interaction matrix
│   └── user_metadata.csv           # Includes simulated gender, age, and region
├── configs/
│   └── movie_config.yaml           # RecBole configuration
├── notebooks/
│   └── Movie_Rec_Fairness.ipynb
├── outputs/
│   ├── log/
│   └── recbole_output/
├── fairness/
│   └── metrics_summary.csv
├── README.md
└── requirements.txt
```

### 🔄 Path Usage Guidelines

- Use **relative paths** (e.g., `./data/movie_ratings.csv`) in code for portability
- Ensure all required folders exist before saving outputs

---

## 📊 Dataset Description

This project uses two datasets:

1. `movie_ratings.csv` – user-movie interaction data (ratings or watch history)
2. `user_metadata.csv` – demographic info including simulated gender for fairness analysis

These are preprocessed to be RecBole-compatible.

---

## 🚀 How to Run

1. **Clone this repository**
```bash
git clone https://github.com/your-username/movie-recbole-fairness.git
cd movie-recbole-fairness
```

2. **Install dependencies**
```bash
pip install -r requirements.txt
```

3. **Launch the notebook**
Open `notebooks/Movie_Rec_Fairness.ipynb` in Jupyter or your IDE.

---

## ✅ Results

- Visualized movie genre popularity skew
- Assessed demographic disparities in top-N recommendations
- Computed AIF360 fairness metrics (e.g., disparate impact, statistical parity)

---

## 📄 License

MIT License

---

## 🤝 Acknowledgements

- [RecBole](https://github.com/RUCAIBox/RecBole)
- [AIF360](https://github.com/Trusted-AI/AIF360)
- [MovieLens](https://grouplens.org/datasets/movielens/) – possible dataset source
