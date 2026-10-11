# Jak utrzymujemy porządek w SNB

**Dla osób aktualizujących zawartość.** Jeśli chcesz tylko przeczytać o wyjazdach, zacznij od [strony głównej](../README.md). Nie trzeba znać GitHuba ani sposobu edycji, żeby korzystać z planów.

## Najważniejsza zasada: piszemy dla uczestników wyjazdu

- Na stronach wyjazdów używamy **zwykłego, zrozumiałego języka polskiego**. Unikamy określeń takich jak `master-plan`, `status`, `checkpoint`, `milestone`, `gate`, `source of truth`, `model kosztowy`, `shortlista` czy `readback`.
- Nazwy ofert, ośrodków i własne określenia organizatora można zachować, ale w razie potrzeby wyjaśniamy je prostym językiem (np. „BUDGET — starsze, tańsze apartamenty”).
- Strony dla uczestników powinny odpowiadać na pytania: **dokąd jedziemy, kiedy, ile to kosztuje, co już ustaliliśmy i co dalej?**
- Zastępujemy nieaktualne informacje w ich dotychczasowym miejscu, zamiast dopisywać kolejny dziennik rozmów, wersje analiz czy datowane podsumowania.
- Jedną informację szczegółowo opisujemy tylko raz. Z innych miejsc podajemy do niej link.
- **„Rozważamy” nie znaczy „wybraliśmy”, a „wybraliśmy” nie znaczy „zarezerwowaliśmy”.** Nie dopisujemy ustaleń, których nie było.
- Zachowujemy źródła ofert, datę sprawdzenia, wymagane dopłaty, istotne zastrzeżenia i powody wyboru. Upraszczamy język, **nie usuwamy ważnych szczegółów**.

## Gdzie umieszczamy informacje

- `README.md` — strona powitalna i odnośnik do aktualnego wyjazdu.
- `wyjazdy/README.md` — wykaz lat, w których planujemy lub odbyliśmy wyjazdy.
- `wyjazdy/<rok>/README.md` — lista wyjazdów z konkretnego roku.
- `wyjazdy/<rok>/<nazwa-wyjazdu>/README.md` — aktualne ustalenia, propozycje i następny krok.
- `wyjazdy/<rok>/<nazwa-wyjazdu>/porownanie-ofert.md` — ceny, daty i warunki wyjazdów.
- `kraje/<kraj>/README.md` — kraj i lista opisanych miejsc.
- `kraje/<kraj>/<osrodek>/README.md` — sam ośrodek lub połączony obszar narciarski.
- `porownania/kraje.md` i `porownania/osrodki.md` — zestawienia zbiorcze z linkami do opisów.
- Kolejny plik (np. `budzet.md` lub `plan-dnia.md`) dodajemy dopiero, gdy uprości on korzystanie z materiałów. Nie tworzymy pustych katalogów na zapas.

Informacje o miejscach przechowujemy pod `kraje/`, a sezonowe terminy, ceny, noclegi i liczbę dni karnetu pod `wyjazdy/`. Porównania mają prowadzić do istniejących opisów bez kopiowania ich całej treści. Przy danych o długości tras zawsze podajemy źródło i zakres karnetu.

**Kierunek odnośników:** strony wyjazdów linkują do krajów i ośrodków, ale strony w `kraje/` i `porownania/` nie linkują z powrotem do `wyjazdy/`. Każda strona z informacjami pochodzącymi ze źródeł zewnętrznych — także w `wyjazdy/` — zawiera jednolity blok daty odczytu, źródła i zakresu według [zasad dat odczytu](zasady-dat-odczytu.md).

Po zakończeniu wyjazdu zachowujemy jego stronę. Nowy wyjazd dostaje **osobny katalog we właściwym roku**. Rok ustalamy według planowanego terminu rozpoczęcia głównego wyjazdu; wyjazdu na przełomie lat nie dzielimy między dwa foldery. Z głównej listy przechodzimy do roku, a następnie do wyjazdu.

## Jak wprowadzamy zmiany na GitHubie

*Poniższe zasady dotyczą tylko redagowania zawartości, nie są instrukcją dla uczestników.*

- Gałąź `main` zawiera obowiązującą, zaakceptowaną wersję stron. Zmiany przygotowujemy na osobnej gałęzi (`branch`), nie zapisujemy bezpośrednio do `main`.
- Każdą spójną zmianę zgłaszamy jako **pull request (PR)** i przeglądamy przed połączeniem. **Draft PR** nie oznacza decyzji ani zatwierdzenia oferty.
- Przed połączeniem sprawdzamy zmienione pliki (`diff`), linki, daty, ceny, brak powtórzeń oraz rozróżnienie ofert proponowanych, wybranych i zarezerwowanych.
- Do `main` preferujemy połączenie typu **squash merge** — jeden commit na PR, chyba że kilka ma uzasadnienie. Bez bezpośrednich zapisów, force-push i przepisywania historii `main`.
- Opis PR jest krótki: **co zmieniono, dlaczego, co nadal trzeba ustalić i co sprawdzono**. Nie kopiujemy przebiegu rozmów i kolejnych prób.
- Jeśli istnieją niejasności, nie zgadujemy i nie ukrywamy ich. Zostawiamy jasne „do sprawdzenia”.

## Prywatność

SNB jest publiczne. **Nie umieszczamy** nazwisk i kontaktów uczestników, danych dokumentów, numerów rezerwacji, informacji o płatnościach, rachunków ani poufnych ustaleń. Takie informacje przechowujemy poza SNB.
