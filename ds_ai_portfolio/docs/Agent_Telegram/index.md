## Agent – Multi-Tool AI Assistant in Telegram 🤖
Node.js | Gemini 1.5 Pro | OpenAI | Telegram Bot API | Google APIs | Notion

Mój asystent AI jest zawsze pod ręką — dosłownie. Wystarczy otworzyć Telegram i napisać, co trzeba zrobić.

Agent rozumie tekst, głos i wideo. Wiadomość głosowa trafia do Whisper, zostaje zamieniona na tekst i wędruje dalej do mózgu systemu — modelu Gemini 1.5 Pro. Ten decyduje, które narzędzie uruchomić: czy wysłać maila, wpisać wydarzenie do kalendarza, stworzyć zadanie, wrzucić notatkę do Notion, wygenerować obraz, policzyć, poszukać w sieci. Każda rozmowa ma pamięć — agent wie, co mówiłeś wcześniej.

To mój codzienny interfejs do własnej produktywności. Bez przełączania aplikacji, bez logowania — jedno miejsce, jeden język naturalny.

Czego się nauczyłem

Architektura agentyczna — jak zbudować system, w którym LLM samodzielnie wybiera narzędzia na podstawie intencji użytkownika <br />
Tool calling w praktyce — definiowanie narzędzi w formacie Gemini, obsługa wywołań zwrotnych i parsowanie wyników <br />
Integracje API — Gmail (nodemailer + Google OAuth), Google Calendar, Google Tasks, Notion API, Perplexity, DALL-E <br />
Multimodalność — obsługa trzech typów wejścia (tekst / głos / wideo) z ujednoliconym pipeline'em przez Whisper <br />
Memory management — Window Buffer Memory dla zachowania kontekstu rozmowy między wiadomościami