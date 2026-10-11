# Movie Recommendation System

A notebook-based recommendation experiment using the MovieLens 100K ratings data. The notebook constructs a user–movie ratings matrix and explores user-based collaborative filtering, item-based collaborative filtering, and Truncated SVD.

## Project files

```text
.
├── LV_2_Task_5.ipynb
├── ml-100k.zip
└── README.md
```

The notebook reads `u.data` and `u.item` from the MovieLens archive. It contains an unzip step; keep `ml-100k.zip` in the repository root and run the notebook from that directory.

## Workflow

1. Extract and load MovieLens 100K ratings and movie metadata.
2. Build a user–item ratings matrix.
3. Calculate cosine similarity for collaborative filtering.
4. Generate recommendations and evaluate a held-out split using Precision@K.
5. Explore item-based collaborative filtering and Truncated SVD recommendations.

## Requirements

The notebook uses Python, Jupyter, pandas, NumPy, Matplotlib, Seaborn, and scikit-learn.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook
```

Open `LV_2_Task_5.ipynb` and run the cells in order. Verify the extracted `ml-100k/ml-100k/` paths if the archive extraction layout differs in your environment.

## Scope and limitations

This repository is an educational notebook, not a deployed recommendation service. The evaluation results depend on the split and metric implementation in the notebook; no recommendation-quality claims are made here.
