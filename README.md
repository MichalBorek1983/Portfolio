# 👨‍💻 Michał Borek – Data Science & AI Portfolio

![Status](https://img.shields.io/badge/Status-Active-success)
![Build](https://img.shields.io/badge/Build-MkDocs-blue)
![Python](https://img.shields.io/badge/Python-3.x-yellow)

> **To repozytorium zawiera kod źródłowy mojego portfolio.**
> ### 🚀 Zobacz pełną wersję online:
> ### 👉 [michalborek1983.github.io/Portfolio](https://michalborek1983.github.io/Portfolio/)

---

## 📄 O mnie
Jestem pasjonatem danych i programowania, który specjalizuje się w przekuwaniu surowych informacji w konkretne rozwiązania biznesowe. Moje portfolio skupia się na praktycznym zastosowaniu **Machine Learningu**, **sztucznej inteligencji (LLM)** oraz **automatyzacji**.

To repozytorium służy do generowania mojej strony wizytówki przy użyciu **MkDocs** i **GitHub Pages**.

---

## 🌟 Wybrane Projekty

Poniżej skrót najważniejszych projektów (te same, co w sekcji "Wyróżnione" na stronie). Pełne opisy znajdziesz online.

### 1. Combined Studio 🎬
**Platforma do produkcji wideo AI** ([emndr.com](https://emndr.com/))
* **Cel:** Cały tor od wyszukania historii po gotowy film, Shorty i materiały marketingowe w jednej aplikacji desktopowej.
* **Tech:** Python, customtkinter, OpenAI, Anthropic, DeepSeek, Groq, Gemini, ElevenLabs, FFmpeg.

### 2. Agenci SDLC 🛡️
**Agenci wspierający cykl życia oprogramowania z kontrolą jakości i bezpieczeństwa**
* **Cel:** Zatrzymywać słabe wyniki agentów, zanim człowiek zacznie je czytać (maszyna stanów, punkt egzekwowania polityki, niezmienny dziennik audytu, brama jakości na zbiorze wzorcowym).
* **Tech:** Python, LangGraph, Claude Agent SDK, SQLite, MCP.

### 3. [AI Decision Helper 🧠](https://decisionhelper.pl/)
**Interaktywne mapy myśli z AI**
* **Cel:** Wizualizacja procesów decyzyjnych przez mapy myśli generowane przez LLM o stałym formacie odpowiedzi.
* **Tech:** React, Node.js, Express, OpenAI API, Groq, ReactFlow.
* 👉 **[Zobacz aplikację live](https://decisionhelper.pl/)**

### 4. Market Opportunity Discovery 🔎
**System oceny nisz rynkowych (prototyp)**
* **Cel:** Cykliczne wyszukiwanie i scoring nisz z siedmiu źródeł, z novelty-check w dwóch etapach (embedding i LLM).
* **Tech:** Python, PostgreSQL, pgvector, Alembic.

### 5. Agent Platform 🏗️
**Prototyp person AI z jawną informacją, że są AI**
* **Cel:** Persony znajdują wątki i piszą odpowiedzi, a człowiek je zatwierdza. Granice bezpieczeństwa są w kodzie, nie w prompcie. Prototyp, jeszcze niewdrożony.
* **Tech:** Python, FastAPI, LangGraph, PostgreSQL, pgvector, Redis, Celery.

### 6. Halfmarathon Predictor 🏃
**Model ML i aplikacja webowa**
* **Cel:** Przewidywanie czasu półmaratonu z komentarzem LLM monitorowanym w Langfuse. [Kod](https://github.com/MichalBorek1983/halfmarathon).
* **Tech:** Python, PyCaret (CatBoost), Streamlit, Langfuse.

### 7. EMNDR Dashboard 📊
**Raport Power BI**
* **Cel:** 10-stronicowy interaktywny raport na zbiorze Contoso: ETL w Power Query, model gwiazdy, miary DAX.
* 👉 **[Zobacz dashboard live](https://app.powerbi.com/links/OiKYGT1Uf7?ctid=ceb753a3-a9ce-4680-857b-99f909b921e3&pbi_source=linkShare&bookmarkGuid=56547e35-0cc8-468d-a7a2-436bce6500c3)**

### Analizy EDA i archiwum
Analizy Iris i Titanic oraz wcześniejsze projekty (Agent Telegram, Audio-Notatki, NaszGPT, Find Friends, Data Integrator) są na stronie w sekcjach "Analizy EDA" i "Archiwum".

---

## 🛠️ Technologie i Narzędzia
W moich projektach wykorzystuję sprawdzony stack technologiczny:

* **Języki:** Python, SQL
* **Data Science:** Pandas, NumPy, Scikit-Learn, Matplotlib/Seaborn
* **AI/LLM:** OpenAI API, LangChain, Whisper
* **Deployment:** Git, Docker, Streamlit, DigitalOcean, GitHub Pages

---

## 📂 Struktura Repozytorium
Dla osób chcących przeanalizować kod źródłowy tej strony:

* `ds_ai_portfolio/mkdocs.yml` - Plik konfiguracyjny generatora strony.
* `ds_ai_portfolio/docs/` - Katalog zawierający pliki Markdown (`.md`) z treścią portfolio.
* `ds_ai_portfolio/docs/assets/` - Obrazy.
* `ds_ai_portfolio/docs/stylesheets/` - Style CSS.

Podgląd lokalny: `pip install mkdocs mkdocs-material`, potem `cd ds_ai_portfolio` i `mkdocs serve`.

---
*Dziękuję za odwiedziny!*
*Jeśli masz pytania lub propozycję współpracy, skontaktuj się ze mną przez [LinkedIn](https://www.linkedin.com/in/micha%C5%82-borek-157258394/) lub e-mail (zakładka Kontakt na stronie).*
