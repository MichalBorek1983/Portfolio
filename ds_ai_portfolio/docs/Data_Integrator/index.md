
#  Data Integrator: Most między cyfrowymi światami
W idealnym świecie wszystkie dane firmy znajdują się w jednej, uporządkowanej bazie. Ale rzeczywistość biznesowa to często chaos: informacje o klientach zamknięte w SQL, katalogi produktów w plikach Excel/CSV, a kluczowe dane finansowe – uwięzione na obrazkach i skanach faktur (PNG).

Ten projekt to odpowiedź na ten chaos. To rurociąg danych (pipeline), który działa jak uniwersalny tłumacz, łączący trzy niekompatybilne ze sobą światy w jedną spójną całość.

Proces integracji odbywa się na trzech płaszczyznach:

Wydobycie (Extraction): System łączy się z bazą SQLite, by pobrać ustrukturyzowane dane klientów. Równolegle parsuje surowe pliki CSV z magazynem produktów. Największe wyzwanie to jednak trzecie źródło – obrazy faktur. Aplikacja musi "przeczytać" pliki graficzne, wydobywając z nich kluczowe liczby i identyfikatory zamówień.

Transformacja (Transformation): Surowe dane są czyszczone, standaryzowane i walidowane. Algorytm dba o to, by ID klienta z bazy pasowało do tego na fakturze, a nazwy produktów były spójne we wszystkich źródłach.

Ładowanie (Loading): Wynikiem działania nie jest kolejny raport do "odkręcania", ale czysty, zunifikowany plik CSV. To "jedno źródło prawdy" (Single Source of Truth), gotowe do natychmiastowej analizy biznesowej.

Ten projekt udowadnia, że format danych nie jest ograniczeniem. Niezależnie od tego, czy informacja jest rekordem w bazie, czy pikselem na skanie faktury – zostanie przetworzona, połączona i dostarczona w użytecznej formie.