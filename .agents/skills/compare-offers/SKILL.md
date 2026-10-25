---
name: compare-offers
description: Analizuj i aktualizuj porównania ofert konkretnego wyjazdu w SNB — daty, ceny, noclegi, karnety, dopłaty i warianty. Nie używaj do ogólnego porównania ośrodków niezależnego od terminów i organizatora.
---

# Porównywanie ofert wyjazdowych

## Zakres i dane wejściowe

1. Ustal, którego wyjazdu i organizatora dotyczy analiza; otwórz jego `README.md` i `porownanie-ofert.md`, jeżeli istnieje. Nie mieszaj ofert z różnych wyjazdów bez wskazanego celu.
2. Zbierz wskazane przez użytkownika oferty lub sprawdź katalog i karty organizatora. Dla każdej pozycji ustal, które dane zweryfikowano, kiedy i w jakim źródle.
3. Rozróżniaj fakty o miejscu od warunków sezonowej oferty. Liczbę kilometrów i charakter terenu weryfikuj z profilem w `kraje/` oraz operatorem; zakres karnetu z kartą konkretnej oferty.
4. Jeśli źródło jest niedostępne lub dane nie zgadzają się ze sobą, napisz „Do sprawdzenia” z wyjaśnieniem; nie przyjmuj najniższej ceny lub szerokiego karnetu bez potwierdzenia.

## Sposób porównania

- Porównuj przynajmniej te cechy, które mają znaczenie dla decyzji i występują w źródłach: nazwa/link oferty, ośrodek/link do profilu, daty wyjazdu, **rzeczywista liczba dni karnetu**, grupa docelowa, rodzaj noclegu i cena wyjściowa z walutą.
- Oddziel **cenę „od”**, obowiązkowe dopłaty, wariant pokoju i warunek jego obłożenia, dodatkowe usługi, koszt transportu, ubezpieczenie oraz **zwrotną kaucję**. Kaucja nie jest końcowym kosztem, jeżeli zostanie zwrócona.
- Kwot w różnych walutach nie dodawaj bez jawnego, uzasadnionego kursu i daty przeliczenia. Nie przedstawiaj kosztu minimalnego jako gwarantowanej ceny dla dowolnej liczby osób.
- Odróżniaj daty podróży od dni jazdy. Nie zakładaj, że dana grupa, transport, miejsce wyjazdu lub opcja noclegu jest dostępna we wszystkich terminach.
- Pilnuj kompletności zestawienia: liczbę ofert i podziały na kraje licz z bieżących pozycji, a nie z historycznego podsumowania. Jeśli szczegółowe koszty policzono tylko dla części ofert, wyraźnie zaznacz zakres, aby nie tworzyć pozornego pełnego rankingu.
- Rekomendacje uzależniaj od jawnych kryteriów użytkownika (np. budżet, dojazd, wielkość terenu). Niewyjaśnionych lub niespójnych warunków nie traktuj jak wad ani zalet potwierdzonych.

## Zapis i aktualizacja

- Dokument z ofertami trzymaj pod `wyjazdy/<rok>/<wyjazd>/porownanie-ofert.md`. Na stronie `README.md` wyjazdu pozostaw podsumowanie i link do szczegółów; nie duplikuj tabel.
- Uporządkuj informacje po krajach lub innym kryterium ułatwiającym decyzję, zachowując linki do oryginalnych kart ofert i profili ośrodków. Nie zmieniaj opisów ośrodków na podstawie samych marketingowych kart ofert.
- Uaktualniaj istniejące sekcje zamiast tworzyć dziennik kolejnych analiz. Zachowaj istotne zastrzeżenia, źródła i powody wniosków.
- Stosuj [zasady dat odczytu](../../../.github/zasady-dat-odczytu.md): przy różnych terminach sprawdzenia źródeł rozdziel daty; nie zastępuj ich automatycznie dzisiejszą datą.
- Jeżeli analiza zmienia ustalenia o wyjeździe, zastosuj także [manage-trips](../manage-trips/SKILL.md). Weryfikuj zgodność podsumowań, liczb ofert, linków, walut i dni karnetu.

## Kontrola i PR

Przed publikacją sprawdź zakres względem `main`, poprawność oferty–ośrodka, dat, dopłat i zastrzeżeń, brak twierdzeń o niepotwierdzonej rezerwacji oraz brak danych prywatnych. Przy zmianach plików stosuj [pull-request](../pull-request/SKILL.md); nie merguj bez polecenia.
