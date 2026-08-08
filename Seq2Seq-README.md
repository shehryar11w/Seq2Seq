# Seq2Seq — English to French Translation

An **encoder-decoder (sequence-to-sequence)** machine translation model trained on English–French sentence pairs, implemented both with and without an **attention** mechanism.

## Contents

| Notebook | Description |
|---|---|
| `seq2seq-plain.ipynb` | A plain encoder-decoder Seq2Seq model without attention. |
| `seq2seq-att.ipynb` | The same task with a Bahdanau/Luong-style attention mechanism added to the decoder. Includes the full preprocessing pipeline: tokenizing text, building vocabularies (word-to-index / index-to-word), adding SOS/EOS tokens, padding, and a custom `collate_fn`/`Dataset`/`DataLoader` with a 90/10 train/test split. |

## Dataset

English-French sentence pairs (`data/fra.txt`), tokenized and split into train/test sets.

## Technologies

- Python
- PyTorch

## Getting Started

```bash
git clone https://github.com/shehryar11w/Seq2Seq.git
cd Seq2Seq
pip install torch
```

Open either notebook in Jupyter or VS Code and run.

## Learning Outcomes

- Building an encoder-decoder architecture for sequence generation from scratch
- How attention improves translation quality over a plain Seq2Seq baseline
- Text preprocessing for NLP: tokenization, vocab building, padding, batching

## License

Educational / personal use.
