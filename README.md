# MineToday 2026 — AI Course Advisor

IT Today IPB 2026, Team cupuu — ranks which learning module a student needs next, from
chat and assessment signals.

## Open this first
- [`cupuu_notebook.ipynb`](./cupuu_notebook.ipynb) — the full pipeline, one notebook:
  setup → business understanding → data understanding/preparation → feature engineering →
  modeling → evaluation → save/load → prediction.

## Approach
LightGBM regression + LambdaRank, bagged across 5 seeds, tuned with 50 Optuna trials,
validated with a 5×3 repeated K-fold (15 folds).

## Result
NDCG@5 (CV) **0.6656**.

No dataset is committed here.
