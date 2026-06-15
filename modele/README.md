# Modele

Wagi RoBERTa-large fine-tuned na LIAR. Pliki `.pt` (~1.3 GB każdy) **nie są** w gicie — siedzą jako assety w GitHub Release.

## Pobieranie

```
gh release download v1.0 --repo juliaprzezdzik/fake-news-detector -D modele/
```

albo ręcznie: https://github.com/juliaprzezdzik/fake-news-detector/releases

## Załadowanie modelu

```python
import torch
from transformers import RobertaForSequenceClassification

model = RobertaForSequenceClassification.from_pretrained('roberta-large', num_labels=2)
model.load_state_dict(torch.load('modele/roberta_large_2cl_baseline.pt'))
model.eval()
```

Dla `roberta_large_6cl_optuna.pt` ustaw `num_labels=6`.
