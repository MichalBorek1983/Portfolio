## Halfmarathon Predictor 🏃
Python | PyCaret (CatBoost) | Streamlit | OpenAI | Langfuse

Każdy biegacz na starcie pyta siebie, na co go stać. Aplikacja przewiduje czas półmaratonu na podstawie płci, wieku i czasu na 5 km, a model językowy dodaje komentarz taktyczny.

### Dane i model

Model regresji powstał na 17 626 wynikach z Półmaratonu Wrocławskiego (edycje 2023 i 2024). Metadane zapisane przy modelu to eksperyment "EXP1" z czasami na 5, 10 i 15 km, wiekiem i płcią, średni błąd bezwzględny 1,36 minuty i R² 0,9876.

### Ograniczenie

Aplikacja pyta użytkownika tylko o czas na 5 km, a czasy na 10 i 15 km szacuje stałymi mnożnikami (2,05 i 3,10 razy czas na 5 km). Liczby z metadanych dotyczą modelu z rzeczywistymi czasami pośrednimi, więc nie podaję ich jako dokładności samej aplikacji. Błąd prognozy z samego czasu na 5 km jest nieznany i może być większy.

### Komentarz modelu językowego

LLM analizuje dane wejściowe i podaje spersonalizowane porady taktyczne. Każda interakcja jest śledzona i oceniana w Langfuse.

Kod jest publiczny: [github.com/MichalBorek1983/halfmarathon](https://github.com/MichalBorek1983/halfmarathon). Aplikacja demonstracyjna jest w tej chwili niedostępna.
