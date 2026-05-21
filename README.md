# LLMs and GenAI Assignment

Project notebooks for the 15-class dataset assignment

## Notebooks

| File | Local | Colab |
|------|-------|-------|
| **Q1** — Pretrained models (ResNet18, DenseNet121, VGG19) | `q1.ipynb` | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nelsunnel/LLMs-and-GenAI-Assignment/blob/main/q1.ipynb) |
| **Q2** — Finetune VGG19 | `q2.ipynb` | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nelsunnel/LLMs-and-GenAI-Assignment/blob/main/q2.ipynb) |
| **Q3** — CLIP ViT-B/16 zero-shot | `q3.ipynb` | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/nelsunnel/LLMs-and-GenAI-Assignment/blob/main/q3.ipynb) |

## Data

- `Datasets/dataset/`: 15 classes, ~805 images (organized by class)
- `Datasets/dataset2/`: Annotations (XML) + images
- `Datasets/pathologyData/`: Train/test split data

## Quick Setup

### Local (Jupyter/VS Code)

1. Create a virtual environment and install requirements:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2. Open the notebooks in Jupyter / VS Code and run cells.

### Google Colab

Click one of the **Colab** badges above. The notebooks will:
1. Auto-detect Colab and install dependencies
2. Clone the repo to access the dataset
3. Run directly on GPU (if available)

No additional setup needed—just click and run!

## Notes

- Notebooks include scaffolding with commented examples to avoid accidental long runs. Adjust `epochs` and uncomment training calls for full experiments.
- For CLIP zero-shot, `git+https://github.com/openai/CLIP.git` is included in `requirements.txt`.
- Colab uses the repo dataset directly via `git clone`; local runs expect `Datasets/` in the workspace root.
