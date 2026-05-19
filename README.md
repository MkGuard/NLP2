# NLP Assignment 2 — Language Modelling

Comparison of n-gram and neural language models trained on *Pride and Prejudice* (Jane Austen).

## Models

| Model | Test Perplexity |
|-------|----------------|
| Trigram (Laplace smoothing) | 2715 |
| CNN LM | 529 |
| LSTM LM (weight tying) | 235 |

## Project Structure

```
NLPAssign2/
├── notebooks/
│   ├── FINAL_ONE_NOTEBOOK.ipynb   # Full pipeline in one notebook
│   ├── notebook1.ipynb            # Data prep & trigram model
│   ├── notebook2.ipynb            # CNN language model
│   ├── notebook3.ipynb            # LSTM language model
│   ├── notebook4.ipynb            # Interpretability & analysis
│   ├── Pride_and_prejudice.txt    # Source corpus
│   ├── requirements.txt
│   └── *.png / *.csv / *.txt      # Plots and analysis outputs
├── models/                        # Saved model weights (not tracked by git)
└── reports/                       # PDF reports
```

## Setup

```bash
pip install -r notebooks/requirements.txt
```

Then open `notebooks/FINAL_ONE_NOTEBOOK.ipynb` in Jupyter.

> **Note:** Model weights (`models/*.h5`) are excluded from the repo due to file size. Re-run the notebook to regenerate them.

## Tasks Covered

1. **Data Exploration** — tokenisation, vocabulary construction, frequency analysis
2. **Trigram LM** — Laplace-smoothed trigram model with text generation
3. **Neural LMs** — CNN and LSTM models with perplexity comparison and learning curves
4. **Interpretability** — gradient-based token importance, embedding visualisation
