## Combined Studio 🎬
Python | customtkinter | OpenAI | Anthropic | DeepSeek | Groq | Gemini | ElevenLabs | FFmpeg

Film na YouTube to dziesiątki narzędzi i zakładek: pomysł, research, skrypt, obrazy, głos, muzyka, montaż, publikacja. Combined Studio zamyka cały ten tor w jednej aplikacji desktopowej, od wyszukania historii po gotowy film, Shorty i materiały marketingowe.

Combined Studio napędza EMNDR, moją markę produkcji wideo AI. Strona studia: [emndr.com](https://emndr.com/).

Skala (stan z 27.09.2026): 97 modułów w Pythonie (ok. 61 tys. linii), 44 pliki testów (ok. 4,6 tys. linii) i 36 raportów audytu kodu.

### Co obejmuje

* **Odkrywanie materiału.** Wyszukiwanie historii i tematów z oceną (scoring), tracker konkurencji z metrykami kanałów i analizą luk, prawdziwa transkrypcja YouTube w trzech warstwach napisów oraz Whisper na audio. Wcześniej model zmyślał treść na podstawie tytułu, więc transkrypcja stała się osobnym krokiem.
* **Redakcja.** Redakcja antyplagiatowa (Claude, z zapasem na DeepSeek), pamięć wcześniejszych redakcji jako lista zakazana (imiona, schematy, otwarcia, metafory), strażnik gramatyki i strażnik wyjścia modelu wykrywający ucięcia.
* **Obrazy.** Podział skryptu na sceny, Style Bible z kotwicą obrazową, trzy silniki obrazu (GPT Image, FAL FLUX, Gemini) wybierane wg ważności sceny oraz wykrywanie niemal identycznych obrazów hashem percepcyjnym.
* **Głos i dźwięk.** Cztery silniki TTS na wspólnej bazie (walidacja, cache SHA-256, kontrola budżetu przed wywołaniem, ponawianie, koszt per fragment), wyrównanie scen do audio przez Whisper ze znacznikami słów, sound design i muzyka.
* **Montaż.** Efekty ruchu obrazu liczone w numpy (paralaksa, cząsteczki z okluzją, dolly-zoom), narrator na kamerze i Shorty wycinane z realnych czasów.
* **Publikacja i koszty.** Materiały marketingowe YouTube z krokiem SEO, planer produkcji z prognozą kosztów i kontrola budżetu przed kosztownymi wywołaniami.

### Decyzje i dowody

* **Wielu dostawców AI.** Model jest dobierany do zadania (szybkość, jakość, koszt), a kluczowe kroki mają zapas u innego dostawcy.
* **Uczciwość danych.** Baza startowa konkurencji pochodząca z analizy modelu jest oznaczona jako szacunkowa.
* **Weryfikacja.** Shorty sprawdzono testem na 8 projektach z prawdziwym API, a kod przeszedł audyt opisany w 36 raportach.

Kod jest prywatny, a efekt pracy platformy widać na stronie [emndr.com](https://emndr.com/).
