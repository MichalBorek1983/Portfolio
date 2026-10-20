## Agent Platform 🏗️
Python | FastAPI | LangGraph | PostgreSQL + pgvector | Redis | Celery | Docker

Prototyp systemu person AI, które mają rozmawiać z ludźmi w internecie i jawnie mówić, że są AI. System sam znajduje wątki warte komentarza i pisze propozycję odpowiedzi, a człowiek ją zatwierdza, zanim cokolwiek zostanie opublikowane. Prototyp nie został jeszcze wdrożony ani uruchomiony publicznie.

### Decyzje projektowe

* **Trzy zasady wbudowane w kod, nie w prompt.** Persona nie może twierdzić, że jest człowiekiem (guardrail blokuje to na twardo: regexy i moderacja OpenAI). Nic nie publikuje się samo (każdy szkic czeka na człowieka). Mechanizm ewolucji nie dotyka reguł bezpieczeństwa, więc charakter persony może dryfować, a granice nie.
* **Radar.** Agent wyszukuje wątki, w których persona ma coś do powiedzenia, zamiast odpowiadać na wszystko.
* **Router modeli.** DeepSeek jest głównym silnikiem, a Groq, Anthropic i Gemini działają jako kaskada zapasowa.
* **Koszty pod kontrolą.** Rachunek per persona i per model, hamulec budżetowy, strażnik pilnujący awarii modeli i zmian cen oraz prognoza kosztów.
* **Ewolucja z odwracalnością.** System mierzy dryf charakteru persony, proponuje zmiany i umożliwia powrót do wcześniejszej wersji.
* **Raport dzienny** trafia na Telegram.

### Stan

Prototyp działa lokalnie. Kolejne fazy opisują osobne dokumenty (warstwa persony, cztery persony, router i radar, strażnik i prognozy). Repozytorium jest prywatne.
