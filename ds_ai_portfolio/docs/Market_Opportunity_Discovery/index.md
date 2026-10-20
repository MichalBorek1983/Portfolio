# Market Opportunity Discovery 🔎
Python | PostgreSQL + pgvector | Alembic | OpenAI embeddings | pytest

System cyklicznego wyszukiwania i oceny nisz rynkowych. Szuka w sieci tematów, które mogą być niszami wartymi sprawdzenia, i ocenia je w sposób, który da się powtórzyć i zakwestionować.

## Decyzje projektowe

* **Siedem źródeł kandydatów.** Hacker News, arXiv, Stack Exchange i GitHub działają bez kluczy, a eBay, USPTO i Tavily są podłączone i czekają na poświadczenia. Google Custom Search odrzuciłem (zamknięty dla nowych klientów, wygasa 1.01.2027), a jego adapter usunąłem z kodu.
* **Novelty-check w dwóch etapach.** Embedding (pgvector, `text-embedding-3-small`) zawęża kandydatów, a dopiero potem wynik potwierdza LLM, więc model jest wołany tylko dla wąskiego zbioru.
* **Założenia jawnie nazwane.** Stałe silnika scoringu i maszyny stanów leżą w plikach YAML z oznaczeniami `[ASSUMPTION]` i `[DECISION]` oraz odnośnikiem do dokumentu źródłowego.
* **Izolacja danych.** System działa w dedykowanym schemacie bazy, nigdy w `public`, a migracje pomijają obiekty spoza tego schematu.
* **Testy bez kosztu.** Testy jednostkowe, złote i end-to-end używają zamockowanego LLM. Prawdziwe wywołania są w osobnych skryptach poza `pytest`.

## Stan i ograniczenia

To prototyp (PoC). Nie ma jeszcze harmonogramu cyklicznego ani raportu. Nie sprawdzono też, czy ocena po co najmniej dwóch cyklach odróżnia się od przypisania losowego. To kryterium przejścia do następnej fazy. Repozytorium jest prywatne.
