# Zasady zapisywania dat odczytu informacji

## Gdzie stosujemy

Każda strona w `kraje/` i `porownania/` oraz każdy dokument w `wyjazdy/` zawierający dane zewnętrzne (np. katalog ofert lub opis wyjazdu) zawiera **ten sam blok bezpośrednio pod tytułem**:

```markdown
**Data odczytu:** RRRR-MM-DD  
**Źródło:** [nazwa źródła](https://adres-zrodla)  
**Zakres:** jakie informacje pochodzą z tego źródła
```

W widoku GitHub trzy pozycje występują w kolejnych wierszach; w pliku Markdown na końcu pierwszych dwóch wierszy stawiamy po dwie spacje.

## Co oznacza data

- **Data odczytu** to dzień, w którym faktycznie sprawdzono wskazaną informację u źródła (format ISO `RRRR-MM-DD`). Nie jest to data wyjazdu, zatwierdzenia strony ani ostatniego commita.
- Gdy przenosimy lub redagujemy tę samą informację bez ponownego sprawdzania źródła, **pozostawiamy poprzednią datę**. Nie odmładzamy danych pozorną datą aktualizacji.
- Zmieniamy datę odczytu dopiero po ponownym sprawdzeniu informacji. Jeśli źródła lub sekcje mają **różne daty odczytu**, podajemy osobne daty przy każdej grupie źródeł, zamiast jednej wprowadzającej w błąd.
- **Źródło** prowadzi do zewnętrznej strony zawierającej dane, a nie do innej strony SNB. Można podać kilka źródeł sprawdzonych tego samego dnia; przy opisach ośrodków używamy odpowiednich kart, a przy zestawieniach — katalogu i właściwych kart.
- **Zakres** jasno rozdziela informacje o samym miejscu od warunków konkretnej oferty. Jeśli liczba kilometrów dotyczy podstawowego karnetu jednego organizatora, zaznaczamy to zamiast nazywać ją całkowitą wielkością ośrodka.
- Jeśli odczyt nie jest możliwy, zaznaczamy **„Do sprawdzenia”**, nie wpisujemy dzisiejszej daty jako potwierdzenia.
- Spis własnych wyjazdów bez danych pobranych ze źródeł zewnętrznych nie potrzebuje takiego bloku. Jednak każda strona zawierająca ceny, zakres karnetu, cechy ośrodka albo warunki organizatora powinna go mieć.

## Kierunek odnośników

- `wyjazdy/` → `kraje/` i `porownania/`: **tak** (w tym bezpośrednie linki od konkretnej oferty do ośrodka).
- `kraje/` → podstrony krajów i ośrodków oraz `porownania/`: **tak**.
- `porownania/` → `kraje/` i inne porównania: **tak**.
- `kraje/` lub `porownania/` → `wyjazdy/`: **nie**. Porównania i opisy miejsc nie zależą od trwających przygotowań do konkretnego wyjazdu.
- Link do **zewnętrznej karty organizatora**, z której pochodzą dane o ośrodku, nie jest linkiem zwrotnym do planu wyjazdu w SNB.

Dokumentacja dla czytelników pozostaje po polsku, bez programistycznego żargonu. Ten plik służy osobom redagującym repozytorium.
