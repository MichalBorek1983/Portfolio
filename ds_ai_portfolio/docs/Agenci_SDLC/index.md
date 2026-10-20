## Agenci SDLC 🛡️
Python | LangGraph | Claude Agent SDK | SQLite | pydantic | MCP

Agent piszący kod jest szybki. Trudniej sprawić, żeby słaby wynik został zatrzymany, zanim człowiek zacznie go czytać. Agenci SDLC to platforma agentów wspierających cykl życia oprogramowania (PO/BA, Architect, QA, Coder, Code Reviewer, Security Auditor), w której kontrola jakości i bezpieczeństwa jest częścią architektury.

### Decyzje projektowe

* **Stan projektu jako maszyna stanów.** Przejścia (od `PRD_DRAFT` do `DONE`) opisuje jawna tabela, a para spoza tabeli kończy się wyjątkiem.
* **Reguła programowa zamiast kolejnego wywołania modelu.** Każde działanie agenta o skutkach jest zapisywane jako Action Envelope i oceniane przez punkt egzekwowania polityki (ALLOW, DENY albo REQUIRE_HUMAN). Klasyfikator semantyczny jest świadomie odłożony i zapisany jako jawnie zaakceptowane ryzyko.
* **Niezmienny dziennik audytu.** Wpisy tworzą łańcuch skrótów, a test zmienia dane surowym SQL i sprawdza, że weryfikacja to wykrywa.
* **Wynik działania z sześcioma stanami** (od `NOT_STARTED` do `FAILED`) zamiast binarnego sukcesu lub porażki.
* **Brama jakości na zbiorze wzorcowym (golden dataset).** Słabe wyjście modelu jest zatrzymywane, zanim trafi do człowieka. Przy jednym przypadku na agenta sygnał okazał się za słaby: ocena architekta wynosiła 1,0, a po rozszerzeniu zbioru do trzech przypadków spadła do 0,33.
* **Router modeli z poziomami i zapasowym dostawcą.** QA i Architect są najpierw kierowani na tańszy model (DeepSeek), z wyższym poziomem jako zapasem.
* **Integracja MCP i interfejs eskalacji.** Orchestrator jest wystawiony jako narzędzie dla Claude Code, a kontrakt kanału eskalacji jest zweryfikowany na żywo. Kanały Slack i WWW są jeszcze w przygotowaniu.

### Stan i dowody

* 426 testów jednostkowych zielonych (pakiet `orchestrator`, stan z dokumentacji faz, wrzesień 2026).
* Bramka GATE-01 (Credential Broker i test negatywny) jest zielona, razem z testem end-to-end na żywym modelu.
* Pełny przebieg na żywym modelu z Security Auditorem był próbowany wielokrotnie. Ukończenia do stanu `DONE` nie potwierdzono, bo zabrakło salda API, a nie z powodu błędu w kodzie.
* Repozytorium jest prywatne, dokumentacja faz jest dostępna na życzenie.
