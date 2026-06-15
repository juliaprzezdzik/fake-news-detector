# Wyniki

Folder na CSV-ki z metrykami modeli + wygenerowane wykresy / macierze pomyłek.

## Format CSV (jeden plik per model)

```
model,wariant,tryb,acc,macro_f1,weighted_f1,precision_macro,recall_macro
roberta-large,2cl,fine-tune,0.738,0.728,0.735,0.737,0.726
gpt-4o,2cl,zero-shot,0.729,0.729,0.730,0.730,0.730
```

`zestawienie_wynikow.ipynb` w katalogu nadrzędnym ładuje wszystkie CSV-ki i generuje wspólne tabele i wykresy.
