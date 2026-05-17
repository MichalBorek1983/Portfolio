## Agent Platform 🏗️
Python | FastAPI | LangGraph | Celery | Redis | PostgreSQL | Qdrant | Docker

Jeden agent AI to projekt. Dziesiątki agentów działających równolegle, z kolejkowaniem zadań, monitoringiem i bazą danych — to już platforma.

Agent Platform to produkcyjna infrastruktura, która pozwala uruchamiać dowolną liczbę agentów LangGraph jako niezależne workery. Zadanie trafia przez REST API do kolejki Celery/Redis, zostaje odebrane przez wolnego workera, agent wykonuje pracę — scrapuje, analizuje, generuje embeddingi — i zapisuje wynik do PostgreSQL. Cały stan jest trwały. Klient może śledzić postęp przez WebSocket w czasie rzeczywistym.

Pod maską: LangGraph definiuje grafy decyzyjne agentów z węzłami i warunkami przejść. Qdrant przechowuje embeddingi do semantycznego wyszukiwania. Langfuse monitoruje każde wywołanie LLM. Alembic zarządza migracjami schematu bazy. Makefile spina wszystko w jeden interfejs CLI.

Czego się nauczyłem

LangGraph — budowanie agentów jako grafów stanów z węzłami decyzyjnymi, pętlami i warunkami przejść zamiast prostego chain-of-thought <br />
Architektura produkcyjna — separacja warstw API / kolejka / worker / baza danych, każda skalowalna niezależnie <br />
Celery + Redis — asynchroniczne kolejkowanie zadań, retry, rate limiting, monitoring przez Flower <br />
FastAPI z WebSocket — streaming wyników do klienta bez pollingu, obsługa wielu równoczesnych połączeń <br />
Docker Compose — orkiestracja pięciu serwisów (API, worker, PostgreSQL, Redis, Qdrant) w jednym pliku <br />
SQLAlchemy + Alembic — modelowanie schematu i zarządzanie migracjami w środowisku produkcyjnym