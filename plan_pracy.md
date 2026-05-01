
## Sprint 0 — Inicjalizacja (17.04 – 20.04 · 6 SP)

Cel: przygotowanie środowiska, wybór tematu i struktury projektu.

| #  | ID    | Typ     | Priorytet  | SP | Zadanie                                                                                                                                |
|----|-------|---------|------------|----|----------------------------------------------------------------------------------------------------------------------------------------|
| 1  | B-001 | Zadanie | Krytyczny | 2  | <code style="color : cyan">+</code> Wybór tematu projektu                                                                              |
| 2  | B-002 | Zadanie | Wysoki    | 1  | <code style="color : cyan">+</code> Założenie repozytorium GitHub (README, .gitignore, licencja)                                       |
| 3  | B-003 | Zadanie | Wysoki    | 2  | <code style="color : cyan">+</code> Konfiguracja środowiska (venv, requirements.txt: transformers, torch, scikit-learn, pandas, spacy) |
| 4  | B-004 | Zadanie | Średni    | 1  | <code style="color : cyan">+</code> Ustalenie struktury katalogów                                                                                                          |

---

## Sprint 1 — Dane (21.04 – 28.04 · 16 SP)

Cel: pozyskanie, eksploracja i przetwarzanie wstępne danych.

| #  | ID    | Typ        | Priorytet  | SP | Zadanie                                                                                                                                    |
|----|-------|------------|------------|----|--------------------------------------------------------------------------------------------------------------------------------------------|
| 5  | B-005 | User Story | Krytyczny | 3  | <code style="color : cyan">+</code> Pozyskanie zbioru danych (min. 1000 przykładów) z udokumentowanym źródłem (KLEJ, PolEval, HF Datasets) |
| 6  | B-006 | User Story | Wysoki    | 5  | <code style="color : cyan">+</code> Eksploracyjna analiza danych (EDA): rozkład klas, długość tekstów, wordcloud, statystyki opisowe       |
| 7  | B-007 | User Story | Krytyczny | 5  | <code style="color : cyan">+</code> Pipeline przetwarzania wstępnego: tokenizacja, normalizacja, lematyzacja (spaCy), czyszczenie          |
| 8  | B-008 | Zadanie    | Wysoki    | 2  | <code style="color : cyan">+</code> Podział danych train/val/test                                                                          |
| 9  | B-009 | Zadanie    | Średni    | 1  | <code style="color : cyan">+</code> Dokumentacja źródła danych w README (źródło, licencja, rozkład klas, format)                                                               |

---

## Sprint 2 — Model klasyczny (29.04 – 06.05 · 13 SP)

Cel: implementacja i ewaluacja podejścia TF-IDF + klasyfikator ML.

| #  | ID    | Typ        | Priorytet  | SP | Zadanie                                        |
|----|-------|------------|------------|----|-------------------------------------------------|
| 10 | B-010 | User Story | Krytyczny | 3  | Ekstrakcja cech: TfidfVectorizer (max_features, ngram_range) |
| 11 | B-011 | User Story | Krytyczny | 5  | Trening modelu klasycznego: Pipeline sklearn (TF-IDF → SVM/NB/LogReg), GridSearchCV |
| 12 | B-012 | User Story | Wysoki    | 3  | Ewaluacja modelu klasycznego: accuracy, precision, recall, F1, confusion matrix, zapis wyników do JSON |
| 13 | B-013 | Zadanie    | Średni    | 2  | Przegląd zgodności kodu z PEP 8 (flake8/pylint, docstrings, ewentualne type hinting konsekwentnie) |

---

## Sprint 3 — Model Transformer (07.05 – 16.05 · 16 SP)

Cel: fine-tuning HerBERT/polish-roberta i ewaluacja.

| #  | ID    | Typ        | Priorytet  | SP | Zadanie                                        |
|----|-------|------------|------------|----|-------------------------------------------------|
| 14 | B-014 | User Story | Wysoki    | 3  | Przygotowanie danych dla Transformera: AutoTokenizer, Dataset class, DataLoader (padding/truncation) |
| 15 | B-015 | User Story | Krytyczny | 8  | Fine-tuning modelu Transformer: HerBERT, HF Trainer, hiperparametry (lr, epochs, batch_size, warmup) |
| 16 | B-016 | User Story | Wysoki    | 3  | Ewaluacja modelu Transformer: te same metryki co model klasyczny, zapis do JSON |
| 17 | B-017 | Zadanie    | Średni    | 2  | Obsługa GPU / optymalizacja: CUDA, gradient accumulation, fp16, checkpointing (opcjonalnie) |

---

## Sprint 4 — Analiza i porównanie (17.05 – 20.05 · 11 SP)

Cel: porównanie ilościowe i jakościowe obu podejść, analiza błędów.

| #  | ID    | Typ        | Priorytet  | SP | Zadanie                                        |
|----|-------|------------|------------|----|-------------------------------------------------|
| 18 | B-018 | User Story | Krytyczny | 3  | Porównanie ilościowe obu podejść: tabela metryk, bar chart F1 per klasa, ROC curves |
| 19 | B-019 | User Story | Krytyczny | 5  | Analiza błędów: typowe pomyłki obu modeli, przykłady źle sklasyfikowanych tekstów, porównanie jakościowe |
| 20 | B-020 | Zadanie    | Wysoki    | 3  | Wizualizacje porównawcze |

---

## Sprint 5 — Dokumentacja i oddanie (21.05 – 25.05 · 15 SP)

Cel: raport techniczny, prezentacja na obronę, finalne oddanie na GitHub.

| #  | ID    | Typ        | Priorytet  | SP | Zadanie                                        |
|----|-------|------------|------------|----|-------------------------------------------------|
| 21 | B-021 | User Story | Krytyczny | 5  | Raport techniczny: problem, dane, metody, wyniki, wnioski  (opcjonalinie) |
| 22 | B-022 | Zadanie    | Wysoki    | 3  | Komentarze w kodzie i notebookach: docstringi modułów i funkcji, komórki markdown |
| 23 | B-023 | Zadanie    | Wysoki    | 2  | Aktualizacja README.md: opis, instalacja, uruchomienie, struktura repo, wyniki |
| 24 | B-025 | Zadanie    | Wysoki    | 2  | Finalny przegląd kodu, requirements.txt, tag v1.0, push — **DEADLINE 25.05.2026** |

