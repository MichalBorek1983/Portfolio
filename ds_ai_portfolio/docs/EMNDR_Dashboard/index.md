## EMNDR Dashboard 📊
Power BI | Business Intelligence | DAX | ETL

Wyobraź sobie, że zarządzasz firmą z siecią sklepów na kilku kontynentach, setkami produktów i milionami transakcji.
Masz dane — ale czy masz **odpowiedzi**?

Dokładnie taki problem chciałem rozwiązać. Zbudowałem interaktywny dashboard analityczny w Power BI, który z chaosu surowych danych robi przejrzysty obraz sytuacji biznesowej — z dynamicznym filtrowaniem na każdym poziomie i widokiem dostosowanym do każdego odbiorcy: analityka, kierownika i zarządu.

EMNDR Dashboard to 10-stronicowy raport oparty na zbiorze danych Contoso (Microsoft), obejmujący pełen cykl: od ETL przez modelowanie, aż po zaawansowane miary DAX i dopracowany UX.

Czego się nauczyłem

**ETL w Power Query** — łączenie tabel z wielu źródeł przez Append Queries, czyszczenie danych (null, błędy, normalizacja tekstów), Split Column dla sklepów <br />
**Star Schema** — model zbudowany od podstaw: tabela kalendarza, relacje 1:* między wymiarami a faktami, dedykowana tabela Miary dla porządku i czytelności <br />
**DAX na czterech poziomach** — podstawowe agregacje z korektą zwrotów, Time Intelligence (YoY, YTD, vs LY z `SAMEPERIODLASTYEAR`), statystyczne (`DISTINCTCOUNT`), kontekstowe (`ALLSELECTED` dla udziałów zachowujących filtry użytkownika) <br />
**Zaawansowany UX w Power BI** — Tooltip z profilem kierownika, parametry pola do przełączania miar na wykresie, bookmarks + nawigacja zakładkowa, formatowanie warunkowe (zielony/czerwony dla YoY)



[![Zobacz Dashboard Live](https://img.shields.io/badge/🚀_Zobacz_Dashboard_Live-7B2FBE?style=for-the-badge)](https://app.powerbi.com/links/OiKYGT1Uf7?ctid=ceb753a3-a9ce-4680-857b-99f909b921e3&pbi_source=linkShare&bookmarkGuid=56547e35-0cc8-468d-a7a2-436bce6500c3)
[![Pobierz prezentację PDF](https://img.shields.io/badge/📄_Pobierz_prezentację_PDF-grey?style=for-the-badge)](EMNDR_Dashboard_Prezentacja.pdf)