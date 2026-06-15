# Fake News Detector — LIAR + RoBERTa

Binary classification of political statements on the LIAR
dataset using RoBERTa fine-tuning.

## Prezentacja

[Pobierz prezentacje projektu](https://github.com/juliaprzezdzik/fake-news-detector/raw/dev/prezka/prezka.pdf)

## Data

[LIAR dataset](https://www.cs.ucsb.edu/~william/data/liar_dataset.zip) — 12,791
labeled political statements from PolitiFact.

## Approach

- Fine-tuning **RoBERTa-base** (`RobertaForSequenceClassification`, 125M params)
- Tokenization: AutoTokenizer (BPE, max_length=128)
- Comparison: raw text vs. classical preprocessing (lowercase, URL/punctuation
  removal)

## Setup

```bash
git clone https://github.com/juliaprzezdzik/fake-news-detector
cd fake-news-detector
python -m venv .venv && source .venv/bin/activate
pip install transformers torch pandas numpy
jupyter notebook fakenewsdet.ipynb
```
