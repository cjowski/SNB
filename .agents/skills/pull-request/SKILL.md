---
name: pull-request
description: Twórz, aktualizuj, przeglądaj i łącz pull requesty we wszystkich obszarach SNB, w tym dokumentacji, opisach krajów, wyjazdach i porównaniach. Użyj przy poleceniach PR, review, popraw, merge lub zmianach plików repozytorium.
---

# Pull requesty w SNB

## Zasady wspólne

Ten skill obejmuje wszystkie zmiany w repozytorium, także w `AGENTS.md`, `.agents/` i `.github/`. Dla danych o miejscach, wyjazdach i ofertach zastosuj także właściwy skill domenowy. Obowiązują [CONTRIBUTING.md](../../../.github/CONTRIBUTING.md), [zasady dat odczytu](../../../.github/zasady-dat-odczytu.md) oraz [szablon PR](../../../.github/pull_request_template.md).

## Przygotowanie i utworzenie PR

1. Ustal intencję, aktualny stan `main` i zakres zmiany. Nie twórz PR dla pytania lub rekomendacji bez polecenia modyfikacji repozytorium.
2. Utwórz osobną gałąź od aktualnego `main`. Nie zapisuj wprost do `main`, nie wykonuj force-push ani nie zmieniaj historii głównej gałęzi.
3. Wprowadź tylko powiązane zmiany. Aktualizuj istniejące treści w ich miejscu, nie twórz wersji historii rozmów. Weryfikuj ścieżki, linki, daty, zakres źródeł i dane prywatne.
4. Przejrzyj diff względem `main`, listę plików i adekwatne testy/kontrole. Raportuj tylko faktycznie uruchomione testy; przy dokumentacji dopuszczalna jest kontrola struktury i linków bez testów automatycznych.
5. Otwórz PR z krótkim opisem: co zmieniono i dlaczego, co zobaczą uczestnicy (jeżeli dotyczy), co sprawdzono, co pozostało niejasne. Użyj istniejącego szablonu sensownie — nie kopiuj checklisty ofert do zmian wyłącznie technicznych.

## Review, poprawki i merge

1. Przy poleceniu **review** odczytaj bieżący PR, diff, komentarze i status; wskaż problemy z lokalizacją i wagą. Nie oznaczaj punktu jako sprawdzonego bez kontroli.
2. Przy poleceniu **popraw** zmień gałąź istniejącego PR, respektując uwagi i zakres, a następnie ponownie sprawdź diff. Nie otwieraj drugiego PR bez potrzeby.
3. Przy poleceniu **merge** upewnij się, że PR dotyczy właściwego repozytorium i ma oczekiwany zakres, że komentarze i uwagi zostały rozpatrzone oraz że nie ma przeszkód do połączenia. Preferuj **squash merge**.
4. **Nie merguj, nie zamykaj PR ani nie przełączaj draft na ready bez wyraźnego polecenia użytkownika.** W razie istotnych wątpliwości wskaż je zamiast udawać gotowość.
5. W odpowiedzi podaj link i stan PR, krótki zakres zmian, wykonane kontrole i niejasności.

## Dodatkowe kontrole treści

- Zrozumiały język na stronach dla uczestników, bez żargonu programistycznego.
- Propozycja ≠ decyzja ≠ rezerwacja. Nie sugeruj potwierdzeń nieobecnych w danych.
- Koszty, zakres karnetu i liczba dni jazdy są porównane według rzeczywistych warunków; źródła i daty odczytu nie są zmyślone.
- Linkowanie nie narusza podziału `wyjazdy/` → `kraje/` i `porownania/`; brak odwrotnych linków do wyjazdów.
- Brak nazwisk, kontaktów, danych rezerwacyjnych, dokumentów i płatności w publicznym repozytorium.
