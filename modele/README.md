# Modele

Folder przeznaczony na wytrenowane modele RoBERTa-large.

## Lokalizacja oryginalna (Google Drive)

`MyDrive/fakenews_cache/`:

- `model_roberta_2cl_roberta-large_lr2e-06_e7_optuna_best/` — RoBERTa-large 2kl + Optuna (best)
- `model_roberta_6cl_roberta-large_6cl_optuna/` — RoBERTa-large 6kl + Optuna
- `model_roberta_6cl_roberta-large_6cl_plus_optuna/` — RoBERTa-large 6kl + LIAR-PLUS

## Struktura każdego folderu modelu

- `config.json` — konfiguracja architektury
- `model.safetensors` — wagi modelu (~1.4 GB)
- `tokenizer.json`, `vocab.json`, `merges.txt`, `special_tokens_map.json` — tokenizer
