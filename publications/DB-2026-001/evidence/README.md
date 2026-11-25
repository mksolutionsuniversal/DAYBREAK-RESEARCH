# DB-2026-001 — publiczna matryca ustaleń

Poniższa matryca stanowi zredagowany indeks ustaleń z dokumentacji badawczej, nie zbiór surowych dowodów. Źródła pozostają w prywatnym archiwum. Nie przeprowadzano ponownej analizy próbek ani surowych logów podczas redakcji.

| ID | Ustalenie | Status i ograniczenie | Źródła |
| --- | --- | --- | --- |
| E01 | Zmiany Cloudflare 8 XI; dwa przebiegi 9 XI. | CONFIRMED, związek przyczynowy nieustalony. | H1a, H2 |
| E02 | Historyczny odmienny łańcuch i ZIP 58 109 740 B. | CONFIRMED | H1a, H2, S12 |
| E03 | Dwie prawdopodobne próby transferu. | PROBABLE; odbiór UNKNOWN. | H1a, H2 |
| E04 | Identyfikacja Stage 1 i odzysk Stage 2. | CONFIRMED statycznie. | S12 |
| E05 | Stage 2 zawiera komunikację i przygotowanie pliku. | CONFIRMED statycznie; rola telemetrii PROBABLE. | S12 |
| E06 | Bezpośrednio pozyskano Mach-O 5 218 432 B. | CONFIRMED; równoważność pełnego łańcucha UNKNOWN. | S3, M2, M3 |
| E07 | Resolver API, 48/53 hashy, kontrole środowiska. | CONFIRMED statycznie; pełne zachowanie runtime UNKNOWN. | S3 |
| E08 | Zweryfikowano dziewięć wpisów konfiguracji x86_64. | CONFIRMED rekonstrukcja; pełne mapowanie UNKNOWN. | S3 |
| E09 | Odzyskano dwa skompilowane bufory OSA. | CONFIRMED statycznie; pełny dispatch UNKNOWN. | S3 |
| E10 | Kod obejmuje zbieranie i komunikację. | CONFIRMED statycznie; wykonanie Stage 4 UNKNOWN. | S3, AUTH |
| E11 | Run 1: zbieranie, archiwizacja, próby POST. | CONFIRMED; treść ZIP i zakończenie UNKNOWN. | R1 |
| E12 | Zbieranie przed pomyślną walidacją hasła. | CONFIRMED w Run 1–2. | R1, R2 |
| E13 | Run 2: osobny artefakt stanu. | CONFIRMED zapis; odbiorca UNKNOWN. | R2, POST, AUTH |
| E14 | Statyczna ścieżka kontroli poświadczenia. | CONFIRMED konstrukcja; szczegółowa interpretacja PROBABLE. | AUTH |
| E15 | Run 2: dwie nieudane i jedna udana kontrola, zapis artefaktu. | CONFIRMED; kolejność w sekundzie UNKNOWN. | R2, POST, AUTH |
| E16 | Dialog i zdarzenia AppleEvents/TCC. | Dialog PROBABLE; zdarzenia CONFIRMED. | R2, N |
| E17 | Pozostałości profilu po Run 2; brak aktywnej próbki w sprawdzonym oknie. | CONFIRMED w zakresie inspekcji; pełna persystencja UNKNOWN. | POST |
| E18 | Run 3: odczyt artefaktu i pomyślna kontrola; zgodne hashe kopii. | CONFIRMED ślady; reużycie PROBABLE. | R3, AUD, M2, M3, N |
| E19 | Zgodność metadanych dwóch artefaktów poświadczenia; obecność ścieżki w ZIP. | CONFIRMED; bezpośredni przepływ UNKNOWN. | M3, AUD |
| E20 | Kopie wybranych magazynów i konfiguracji w Run 2. | CONFIRMED udokumentowane zapisy; pełny ZIP UNKNOWN. | R2 |
| E21 | Notes z WAL/SHM i inne pliki zachowane w Run 3. | CONFIRMED pliki; stan rekordów UNKNOWN. | M3, AUD |
| E22 | Odnaleziono 6/16 znaczników. | CONFIRMED wynik wyszukiwania; dostęp do obiektów UNKNOWN. | R3, AUD, N |
| E23 | Trzy operacje archiwizacji Run 3 i sprzątanie. | CONFIRMED; wcześniejsze ZIP UNKNOWN. | R3, AUD |
| E24 | ZIP 289 526 B, CRC PASS, 61 ścieżek; 38 zgodnych plików, 2 różnice metadanych, 21 AppleDouble. | CONFIRMED porównanie; przyczyna różnic PROBABLE. | R3, AUD, M3 |
| E25 | Próby sieciowe Run 1–2; 59/124 SYN bez zestawienia TCP dla obserwowanego celu. | CONFIRMED w zakresie PCAP. | R1, R2, S3 |
| E26 | Odłączenie WAN według operatora; ruch zgodny z izolacją. | CONFIRMED udokumentowana konfiguracja; otwarta sieć UNKNOWN. | N, R1, R2, M3 |
| E27 | Kontrole integralności 41/42, 43/43, 44/44 i 90/90. | CONFIRMED według raportów; nie dowodzi kompletności. | R1, R2, M2, R3, M3, AUD |
| E28 | Zachowania klasy infostealer; heurystyka sugerująca AMOS. | CONFIRMED klasa; zgodność cech PROBABLE; atrybucja UNKNOWN. | S3, R1, R2, AUD, H1a, H2 |

## Indeks źródeł wewnętrznych (opisy publiczne)

| ID | Zakres |
| --- | --- |
| S12 | Analiza statyczna Stage 1 i 2, identyfikatory i porównanie historyczne. |
| S3 / S3A | Aktualna i wcześniejsza rewizja analizy statycznej Stage 3. |
| R1 | Raport śledczy Run 1. |
| R2 | Raport śledczy Run 2. |
| M2 | Manifest szerszego zestawu Run 2. |
| POST | Inspekcja hosta po Run 2. |
| AUTH | Analiza statyczna ścieżki uwierzytelnienia. |
| R3 | Analiza offline Run 3. |
| M3 | Manifest Run 3. |
| AUD | Końcowy audyt porównawczy Run 3. |
| H1a / H1b | Dwie rewizje raportu incydentu 9 XI. |
| H2 | Historyczny audyt powłamaniowy. |
| N | Dziennik projektu, §1–37. |

Nie publikujemy wartości poświadczeń, ich skrótów, prywatnych adresów archiwum ani szczegółowych ścieżek użytkowników.
