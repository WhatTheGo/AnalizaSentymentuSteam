# Analiza Sentymentu Recenzji Gry Final Fantasy XIII ze Steam

Projekt studencki z zakresu przetwarzania języka naturalnego (NLP).
Celem projektu jest klasyfikacja recenzji gry Final Fantasy XIII z platformy Steam jako pozytywnych lub negatywnych.

## Opis projektu

Na podstawie recenzji użytkowników Steam zbudowano model uczenia maszynowego,
który automatycznie przewiduje sentyment recenzji (pozytywna / negatywna) na podstawie jej treści tekstowej.

## Struktura projektu

Projekt składa się z 3 notatników Jupyter:

1. **01_dane_i_przetwarzanie.ipynb** - Dane i przetwarzanie wstępne
2. **02_modele.ipynb** - Implementacja modeli
3. **03_ewaluacja_i_analiza.ipynb** - Ewaluacja i analiza wyników

## Dane

### Źródło
Zbiór dancyh pobrany z https://www.kaggle.com/datasets/andrewmvd/steam-reviews.
zawiera recenzje z platformy Steam dla prawie 10 000 gier. 
Na potrzeby projektu używane są tylko recenzje dla gry Final Fantasy XIII.
Każda recenzja posiada treść tekstową oraz etykietę określającą czy jest pozytywna, czy negatywna.

### Licencja zbioru danych
`CC BY NC 4.0`

### Rozkład klas w zbiorze
review_score  
$~$1 (pozytywne) $~~$ 2805   
-1 (negatywne) $~$ 1094 

### Format danych

- **Plik:** `steam_reviews.csv`
- **Separator:** `,`
- **Liczba wierszy:** ~160 000
- **Kolumny:**  
  | Kolumna | Typ | Opis |  
  | app_id | int | Id gry |  
  | app_name | string | Nazwa gry |  
  | review_text | string | Treść recenzji |  
  | review_score | int | Ocena (1 = pozytywna, -1 = negatywna) |

## Licencja

MIT License

Copyright (c) [2026] [Michał Bogdański]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Autor

Michał Bogdański
