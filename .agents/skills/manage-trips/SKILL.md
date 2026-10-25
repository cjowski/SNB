---
name: manage-trips
description: Zakładaj i aktualizuj strony planowanych i zakończonych wyjazdów snowboardowych i narciarskich w SNB. Użyj do zapisywania ustaleń, terminów, decyzji i kolejnych kroków; porównanie konkretnych ofert wykonuj z compare-offers.
---

# Zarządzanie wyjazdami

## Rozpoznanie zadania

1. Sprawdź [wyjazdy/README.md](../../../wyjazdy/README.md), odpowiedni rok i istniejącą stronę wyjazdu. Aktualizuj istniejący wyjazd zamiast zakładać duplikat.
2. Wyjazd należy do `wyjazdy/<rok>/<nazwa-wyjazdu>/`; rok wyznacza początek głównego wyjazdu, również gdy termin przechodzi na kolejny rok. Nowy wyjazd dostaje własny katalog, a zakończony pozostaje w repozytorium.
3. Oddziel ustalenia przekazane przez użytkownika od propozycji, danych zewnętrznych i hipotez. Przy braku potwierdzenia pozostaw sprawę otwartą.

## Strona wyjazdu

- `README.md` wyjazdu ma odpowiadać w pierwszej kolejności: dokąd, kiedy, dla kogo w ujęciu organizacyjnym, ile to może kosztować, co ustalono i co dalej. Pisz prostym polskim, bez języka zarządzania projektami.
- Oznaczaj etapy wprost: **rozważamy**, **wybraliśmy**, **zarezerwowaliśmy**. Wybór oferty nie potwierdza automatycznie rezerwacji; opieraj zmianę etapu wyłącznie na dostarczonym potwierdzeniu.
- Dane o terenie kieruj do `kraje/`, a przekrojowe porównania do `porownania/`. Nie kopiuj szczegółowych profili ośrodków na stronę wyjazdu.
- Konkretne oferty, warianty noclegów, ceny i dopłaty porównuj w `porownanie-ofert.md` według [compare-offers](../compare-offers/SKILL.md). Strona główna wyjazdu zawiera krótkie podsumowanie i link.
- Po utworzeniu wyjazdu uzupełnij listę roku (`wyjazdy/<rok>/README.md`), `wyjazdy/README.md` i — jeśli to najbliższy wyjazd — adekwatny odnośnik w głównym `README.md`. Nie zmieniaj statusu innych wyjazdów bez podstawy.
- Dla danych ze źródeł zewnętrznych umieszczaj blok `Data odczytu / Źródło / Zakres` zgodnie z [zasadami dat odczytu](../../../.github/zasady-dat-odczytu.md). Same ustalenia wewnętrzne nie wymagają pozornej daty odczytu zewnętrznego.

## Prywatność i spójność

- SNB jest publiczne. Nie zapisuj nazwisk, adresów, kontaktów, numerów rezerwacji, danych dokumentów, potwierdzeń wpłat ani poufnych ustaleń. Liczebność grupy czy ogólne wymagania można podać tylko wtedy, gdy nadają się do publikacji.
- Zachowuj jedną aktualną wersję ustaleń: poprawiaj treść w miejscu, nie dopisuj historii czatu, nie twórz kolejnych plików z tym samym podsumowaniem.
- Sprawdź nawigację `README.md` → rok → wyjazd, linki do profili i ofert, status ustaleń oraz zgodność z [CONTRIBUTING.md](../../../.github/CONTRIBUTING.md).
- Przy zmianach stosuj [pull-request](../pull-request/SKILL.md). Nie merguj bez wyraźnego polecenia.
