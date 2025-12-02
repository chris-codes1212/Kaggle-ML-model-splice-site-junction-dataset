# 🧬 DNA Splice Junction Machine Learning Classifier

This project builds machine learning models to classify DNA sequences
based on whether they contain key splice junction sites---**Exon--Intron
(EI)**, **Intron--Exon (IE)**, or **Neither**. Using classical ML
algorithms and cross-validation, the work explores how shallow learning
models can detect biologically meaningful splice site patterns within
fixed-length nucleotide sequences.

## 📘 Background

During RNA splicing, introns (non-coding regions) are removed and exons
(coding regions) are joined together. Two key splice junction types
define intron boundaries:

-   **EI Site (Exon → Intron)** --- Marks the end of an exon and the
    start of an intron.
-   **IE Site (Intron → Exon)** --- Marks the end of an intron and the
    beginning of a new exon.

## 🧪 Dataset

Dataset:
https://www.kaggle.com/datasets/muhammetvarl/splicejunction-gene-sequences-dataset

Characteristics: - \~1000 DNA sequences - 60 nucleotides each - 180
encoded features - Labels: EI, IE, N

## 🎯 Goal

Classify sequences into EI, IE, or Neither.

## 🧠 Methods

Models used: - Random Forest - Gradient Boosting - XGBoost

All models tuned with cross‑validation.

## 🔮 Future Work

-   Motif-based features (GT/AG)
-   KBANN
-   Deep learning approaches

## 🛠 Run Instructions

Install:

``` bash
pip install numpy pandas scikit-learn xgboost
```

Run:

``` bash
jupyter notebook
```

## 🤝 Contributions

PRs and issues welcome.

## 📄 License

MIT recommended.
