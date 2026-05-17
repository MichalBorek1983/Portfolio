## Combined Studio 🎬
Python | customtkinter | OpenAI | Anthropic | Groq | YouTube Data API | NBP API

Tworzenie treści na YouTube to kilka godzin pracy rozrzuconej po dziesiątkach zakładek: szukasz pomysłu, oceniasz potencjał, piszesz skrypt, myślisz o produkcji. Combined Studio zamyka to wszystko w jednej aplikacji desktopowej.

Narzędzie działa w dwóch trybach. Story Finder przeszukuje internet i YouTube w poszukiwaniu historii i trendów — każdy wynik trafia do Groq (Llama 3) do szybkiego scoringu, a model ocenia potencjał materiału jako odcinek po polsku. Studio Produkcji przejmuje wybraną historię i przez Claude Sonnet generuje pełny plan produkcyjny: arc narracyjny, kluczowe momenty, sugestie wizualne. Przepisywanie antyplagiatowe obsługuje OpenAI lub Anthropic — do wyboru w locie. Koszty każdego wywołania API są śledzone na bieżąco z przeliczeniem na PLN przez kurs NBP.

Czego się nauczyłem

Multi-provider AI — równoległe korzystanie z OpenAI, Anthropic i Groq w jednej aplikacji, dobieranie modelu do zadania (szybkość vs jakość vs koszt) <br />
Aplikacje desktopowe w Pythonie — budowanie responsywnego GUI w customtkinter z ciemnym motywem, zakładkami i dynamicznymi komponentami <br />
YouTube Data API v3 — wyszukiwanie filmów i kanałów, pobieranie statystyk, filtrowanie po dacie i zasięgu <br />
Cost tracking — śledzenie zużycia tokenów w czasie rzeczywistym z przeliczaniem na PLN przez API NBP <br />
Refaktoryzacja — przeprojektowanie monolitu (jeden plik 1000+ linii) na modularną architekturę warstwową