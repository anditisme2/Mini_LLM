# Mini_LLM

A from-scratch implementation of a Large Language Model in Python, built while following freeCodeCamp's [Create a Large Language Model from Scratch with Python – Tutorial](https://www.youtube.com/watch?v=UU1WVnMk4E8).

Following the tutorial step by step, learning tokenization, embeddings, self-attention, transformer blocks, and how to train a model from raw text data.

## Status

Core tutorial complete: `bigram.ipynb` (baseline) and `gpt.ipynb` (full GPT-style transformer).

## Goals

- Understand how transformer-based language models actually work under the hood
- Implement tokenization, embeddings, attention, and transformer blocks manually
- Train a small GPT-style model on a custom text corpus
- Get comfortable with PyTorch for deep learning

## Tech Stack

- Python 3
- PyTorch
- NumPy
- Matplotlib
- Jupyter Notebook

## Setup

Clone the repo:
```bash
git clone <your-repo-url>
cd <your-repo-name>
```

Create and activate a virtual environment:
```bash
python3 -m venv cuda
source cuda/bin/activate   # macOS/Linux
# cuda\Scripts\activate    # Windows
```

Install dependencies:
```bash
pip3 install -r requirements.txt
```

Register the environment as a Jupyter kernel:
```bash
python -m ipykernel install --user --name=cuda --display-name "Python (cuda)"
```

Launch Jupyter:
```bash
jupyter notebook
```

## Progress / Topics Covered

- [x] Environment setup (venv, CUDA, Jupyter) - `torch_examples.ipynb`
- [x] Data preprocessing & tokenization
- [x] Bigram language model
- [x] Self-attention mechanism
- [x] Multi-head attention
- [x] Transformer blocks
- [x] Training loop & loss tracking
- [x] Text generation from the trained model

## Files

- `torch_examples.ipynb` - PyTorch building blocks (tensors, tril, softmax, embeddings)
- `bigram.ipynb` - character-level bigram baseline
- `gpt.ipynb` - self-attention, multi-head attention, transformer blocks, training, generation
- `sherlock_holmes.txt` - training corpus

## Next steps

- Try a subword tokenizer (BPE / tiktoken) instead of characters
- Scale up `n_embd`, `n_layer`, `block_size` on a GPU
- Add learning-rate scheduling and gradient clipping

## Acknowledgements

- Tutorial: freeCodeCamp.org – Create a Large Language Model from Scratch with Python
- Built for learning purposes, to understand LLM architecture and training from the ground up.

## License

Personal learning project. Feel free to fork and adapt it for your own study.
