# SNB — punkt wejścia dla asystentów AI

SNB jest publicznym zbiorem informacji o ośrodkach narciarskich, porównań oraz planów wspólnych wyjazdów na narty i snowboard. Pracuj po polsku, chyba że użytkownik poprosi inaczej.

## Jak zacząć

1. Na początku rozmowy przeczytaj **wszystkie pliki** w `.github/`. Obecnie są to: [CONTRIBUTING.md](.github/CONTRIBUTING.md), [zasady-dat-odczytu.md](.github/zasady-dat-odczytu.md) i [pull_request_template.md](.github/pull_request_template.md). To wspólne zasady, których skille nie zastępują.
2. Ustal intencję użytkownika i otwórz odpowiedni skill poniżej oraz tylko pliki potrzebne do zadania. Nie wczytuj całego repozytorium bez potrzeby.
3. Traktuj bieżące pliki repozytorium jako źródło jego aktualnego stanu, a sprawdzone źródła zewnętrzne jako podstawę informacji o ofertach i ośrodkach. Nie wymyślaj danych, decyzji, cen, źródeł ani wyników kontroli.
4. Pytania i rekomendacje bez polecenia zmiany repozytorium obsługuj bez tworzenia PR. Jeśli polecenie obejmuje zmianę plików, korzystaj z właściwego skilla domenowego i [pull-request](.agents/skills/pull-request/SKILL.md).

## Zadanie → instrukcja

- **Dodanie lub aktualizacja kraju bądź ośrodka** (trasy, karnety, snowboard, dojazd, opis miejsca): [manage-resorts](.agents/skills/manage-resorts/SKILL.md).
- **Nowy wyjazd lub aktualizacja ustaleń o wyjeździe** (cel, terminy, uczestnicy w ujęciu zbiorczym, kolejne kroki): [manage-trips](.agents/skills/manage-trips/SKILL.md).
- **Porównanie ofert konkretnego wyjazdu** (terminy, ceny, dopłaty, noclegi, organizator): [compare-offers](.agents/skills/compare-offers/SKILL.md).
- **Porównanie krajów lub ośrodków niezależne od wyjazdu**: [compare-resorts](.agents/skills/compare-resorts/SKILL.md).
- **Pytania, wyszukiwanie i rekomendacje bez zapisu**: zacznij od [README.md](README.md), [kraje/](kraje/README.md), [porownania/](porownania/README.md) lub [wyjazdy/](wyjazdy/README.md); weryfikuj aktualność danych, gdy ma to znaczenie.
- **PR, review, poprawki, merge lub inna operacja na repozytorium**: [pull-request](.agents/skills/pull-request/SKILL.md), a przy zmianach merytorycznych także odpowiedni skill powyżej.

## Mapa repozytorium

- [README.md](README.md) — strona wejściowa dla uczestników i odnośnik do najbliższego wyjazdu.
- [kraje/](kraje/README.md) — opisy krajów i ośrodków, niezależne od konkretnego wyjazdu; `kraje/<kraj>/<osrodek>/README.md` to profil miejsca.
- [porownania/](porownania/README.md) — przekrojowe porównania [krajów](porownania/kraje.md) i [ośrodków](porownania/osrodki.md).
- [wyjazdy/](wyjazdy/README.md) — lata i wyjazdy; `wyjazdy/<rok>/<wyjazd>/README.md` to bieżące ustalenia, a `porownanie-ofert.md` to oferty związane z tym wyjazdem.
- [.github/CONTRIBUTING.md](.github/CONTRIBUTING.md) — język, struktura, linkowanie, zasady edycji i prywatności.
- [.github/zasady-dat-odczytu.md](.github/zasady-dat-odczytu.md) — wymagany zapis daty sprawdzenia, źródła i zakresu danych zewnętrznych.
- [.github/pull_request_template.md](.github/pull_request_template.md) — kontrola zmian przed połączeniem.

## Reguły wspólne

- Informacje o samym terenie i ośrodku zapisuj pod `kraje/`. Terminy, ceny, noclegi, dopłaty i warunki konkretnych ofert zapisuj pod `wyjazdy/`. Zestawienia w `porownania/` odsyłają do profili zamiast powtarzać ich treść.
- Zachowuj kierunek linkowania: `wyjazdy/` mogą wskazywać `kraje/` i `porownania/`; `kraje/` i `porownania/` **nie** odsyłają do `wyjazdy/`.
- Przy danych zewnętrznych stosuj blok `Data odczytu / Źródło / Zakres`. Datę zmieniaj wyłącznie po rzeczywistym ponownym sprawdzeniu źródła. Nieaktualne lub niepotwierdzone dane oznaczaj jako „Do sprawdzenia”.
- Rozdzielaj kilometry przygotowanych tras od freeride, pojedynczy ośrodek od szerszego obszaru oraz karnet podstawowy od rozszerzonego. Przy sprzecznych źródłach opisuj różnicę, nie wybieraj liczby arbitralnie.
- Rozróżniaj **rozważaną propozycję**, **wybraną opcję** i **potwierdzoną rezerwację**. Niczego nie przedstawiaj jako uzgodnione bez podstawy w danych lub poleceniu użytkownika.
- Koszty porównuj z uwzględnieniem waluty, obowiązkowych dopłat, warunków pokoju, liczby dni jazdy i oddzielnego charakteru kaucji zwrotnej. Nie dopisuj fikcyjnej dostępności ani kwot końcowych.
- Pisz dla uczestników prostym językiem polskim. Aktualizuj informacje w dotychczasowym miejscu zamiast prowadzić dziennik rozmów lub duplikować opisy.
- Repozytorium jest publiczne: nie zapisuj danych osobowych, danych rezerwacji, płatności ani poufnych ustaleń.
- Zmiany przygotowuj na osobnej gałęzi w PR; **nie merguj bez wyraźnego polecenia**. Weryfikuj diff i linki oraz raportuj tylko faktycznie wykonane kontrole.
