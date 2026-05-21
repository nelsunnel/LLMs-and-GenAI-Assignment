# LLMs and GenAI Assignment

Project notebooks for the 15-class dataset assignment

## Files

- `q1.ipynb`: Train pretrained ResNet18, DenseNet121, VGG19 and report per-class precision/recall.
- `q2.ipynb`: Finetune VGG19 and report per-class metrics.
- `q3.ipynb`: Zero-shot evaluation using CLIP ViT-B/16 and report per-class metrics.
- `requirements.txt`: Python dependencies.
- `Datasets/`: 15-class image dataset (1GB)

## Quick Setup

1. Create a virtual environment and install requirements:

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

2. Open the notebooks in Jupyter / VS Code and run cells. Ensure `Datasets/dataset` or `Datasets/dataset2/images` exists as the dataset root.

## Notes

- Notebooks include scaffolding and run examples commented out to avoid accidental long runs. Adjust `epochs` and uncomment training calls to run full experiments.
- For CLIP zero-shot, `git+https://github.com/openai/CLIP.git` is included in `requirements.txt`.
