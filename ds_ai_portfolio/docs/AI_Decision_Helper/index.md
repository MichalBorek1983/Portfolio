# AI Decision Helper 🧠
React | Node.js | Express | ReactFlow | OpenAI API | Groq

Siedzisz przed ważną decyzją. W głowie masz chaos: dziesiątki myśli, które się przeplatają, argumenty za i przeciw, pytania bez odpowiedzi. Otwierasz notatnik i po godzinie masz ścianę tekstu, ale nadal nie wiesz, co wybrać. Mózg myśli w skojarzeniach i rozgałęzieniach, a tradycyjne notatki tego nie oddają. Dlatego powstała ta aplikacja: wpisujesz temat, a odpowiedź modelu staje się mapą myśli, jednym faktem i trzema gałęziami do rozwinięcia.

## Decyzje projektowe

* **Odpowiedź modelu ma stały kształt.** Kod dzieli ją po separatorze `||` na kod języka, fakt i trzy gałęzie, a z reszty buduje węzły. Gdy zostaną mniej niż dwie części, aplikacja informuje o niepoprawnym formacie i prosi o ponowienie.
* **Każda gałąź ma swoją rolę.** A to alternatywa lub inny przykład z tej samej kategorii, B to strona techniczna, finansowa lub praktyczna, C to kontekst historyczny, społeczny lub ryzyko. Reguły w prompcie wymuszają brak powtórzeń, więc gałęzie otwierają nowe kategorie.
* **Pozycje węzłów liczy klasa na 83 linie.** Dla każdej kolumny trzyma zajęte przedziały pionowe z buforem 50 jednostek, a zajęta pozycja odsyła węzeł na koniec kolumny. Stałe układu są w jednym pliku konfiguracyjnym.
* **Wybór modelu.** `llama-3.3-70b` przez Groq (darmowy), `gpt-4o-mini` i `gpt-4o` z kluczem OpenAI. Rozmowy zapisują się automatycznie.

## Dowód

Działająca aplikacja: [decisionhelper.pl](https://decisionhelper.pl/). Repozytorium jest prywatne.
