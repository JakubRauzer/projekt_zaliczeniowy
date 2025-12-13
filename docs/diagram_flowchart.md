DIAGRAM PRZYPADKÓW UŻYCIA (ASCII)

                +--------------------------------------------+
                |                 System                     |
                |                                            |
                |    (Zaloguj się)                           |
                |                                            |
                |    (Wyślij dane)       (Integracja z API)  |
                |         |---------------------|            |
                |         |                     \           |
                |    (Waliduj i przetwórz dane)  (Synchronizuj dane) |
                |         |                     /           |
                |    (Generuj raport)      (Eksport / Import) |
                |         |                                    |
                |    (Pobierz raport / Eksport)               |
                |                                            |
                |    (Zarządzaj konfiguracją)                 |
                |    (Przeglądaj logi)                        |
                +--------------------------------------------+

Użytkownik (aktor)  ------------->  (Zaloguj się)
                                  -> (Wyślij dane)
                                  -> (Pobierz raport)

Administrator (aktor) ----------->  (Zaloguj się)
                                  -> (Zarządzaj konfiguracją)
                                  -> (Przeglądaj logi)

System zewnętrzny (aktor/API) -->  (Integracja z API)
                                  -> (Synchronizuj dane)
                                  -> (Eksport / Import)

Uwagi:
- Owal oznaczony tekstem w nawiasach = przypadek użycia.
- Akcje użytkowników i administratora wskazane strzałkami do przypadków użycia.
