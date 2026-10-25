---
name: compare-resorts
description: Twórz i aktualizuj przekrojowe porównania krajów i ośrodków narciarskich w SNB, niezależnie od ofert konkretnego wyjazdu. Użyj przy rankingach, zestawieniach tras, karnetów, snowboardu oraz warunków terenowych.
---

# Porównania krajów i ośrodków

## Zakres

1. Sprawdź [porownania/README.md](../../../porownania/README.md), [kraje.md](../../../porownania/kraje.md), [osrodki.md](../../../porownania/osrodki.md) i odpowiednie profile w `kraje/`.
2. Zestawienie krajów opisuje różnice ogólne, a zestawienie ośrodków konkretne parametry terenów. **Terminy, ceny i noclegi ofert wyjazdowych** należą do [compare-offers](../compare-offers/SKILL.md).
3. Bazuj na aktualnych profilach, lecz sprawdzaj ich źródła i daty, gdy porównanie wymaga aktualności. Nie zakładaj, że starsza liczba jest nadal prawdziwa.
4. Gdy brak profilu lub jego dane wymagają korekty, zastosuj również [manage-resorts](../manage-resorts/SKILL.md). Nie dopisuj fikcyjnego miejsca tylko po to, by wypełnić tabelę.

## Porównywalność danych

- Każda pozycja powinna linkować do odpowiedniego profilu w `kraje/`. Nie powielaj długich opisów z profili.
- Porównuj **ten sam rodzaj miary**: długość przygotowanych tras, zakres konkretnych karnetów, wysokości lub udogodnienia snowboardowe. Gdy nie da się uzyskać wspólnej definicji, pokaż wartości z oznaczeniem źródła i zakresu zamiast sztucznego rankingu.
- Oddziel lokalny teren od połączonego regionu, trasy narciarskie od freeride, liczbę wyciągów od liczby tras oraz dostępność podstawową od rozszerzenia karnetu.
- Nie dodawaj kilometrów połączonych ośrodków, jeżeli zostały już policzone jako region. Nie traktuj danych z oferty organizatora jako uniwersalnej cechy ośrodka.
- Ranking lub rekomendację opieraj na nazwanych kryteriach i rzetelnie oznaczaj braki; nie ogłaszaj „najlepszego ośrodka” bez odniesienia do potrzeb i warunków.

## Aktualizacja i kontrola

- Zmieniaj istniejące `porownania/kraje.md` i `porownania/osrodki.md` zamiast tworzyć drugą wersję tej samej tabeli.
- Przy danych zewnętrznych zachowuj blok `Data odczytu / Źródło / Zakres` bezpośrednio pod tytułem zgodnie z [zasadami dat odczytu](../../../.github/zasady-dat-odczytu.md). Różne daty sprawdzenia rozdzielaj, nie odświeżaj ich pozornie.
- Utrzymuj linki `porownania/` → `kraje/`, ale **nigdy** `porownania/` → `wyjazdy/`. Sprawdź, czy liczba porównywanych ośrodków odpowiada liczbie pozycji tabeli.
- Sprawdź spójność tabel z profilami, rozbieżności źródeł, brak duplikatów i przyjazny język; stosuj też [CONTRIBUTING.md](../../../.github/CONTRIBUTING.md).
- Przy zmianach plików stosuj [pull-request](../pull-request/SKILL.md); nie merguj bez polecenia.
