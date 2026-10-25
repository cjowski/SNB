---
name: manage-resorts
description: Dodawaj i aktualizuj opisy krajów i ośrodków narciarskich w SNB, w tym trasy, karnety, snowboard i źródła. Użyj przy prośbach o nowy profil lub aktualizację informacji o miejscu; nie używaj do cen i terminów konkretnych wyjazdów.
---

# Kraje i ośrodki narciarskie

## Cel i źródła

1. Ustal, czy chodzi o profil miejsca, region połączony wspólnym karnetem, czy ofertę konkretnego organizatora. Warunki oferty należą do `wyjazdy/` i [compare-offers](../compare-offers/SKILL.md).
2. Przejrzyj odpowiedni kraj, istniejące profile i [porównanie ośrodków](../../../porownania/osrodki.md), aby uniknąć duplikatu oraz ustalić dotychczasowe nazewnictwo.
3. Weryfikuj istotne informacje w aktualnych źródłach, preferując operatora terenu i oficjalne informacje o karnetach. Karta organizatora może opisywać zakres jego konkretnej oferty, ale nie dowodzi zakresu każdego karnetu.
4. Jeśli źródła są sprzeczne, zapisz wartości z ich atrybucją, różnicę zakresu i to, co nadal wymaga potwierdzenia. Nie wyrównuj danych przez zgadywanie.

## Miejsce i treść

- Kraje mają `kraje/<kraj>/README.md`, a ośrodki `kraje/<kraj>/<osrodek>/README.md`. Zachowaj istniejące nazwy katalogów i konwencję małych liter z myślnikami, bez polskich znaków.
- Zacznij profilem zrozumiałym dla uczestnika: kraj i region, charakter terenu, długość przygotowanych tras w określonym zakresie, wysokości, możliwości snowboardowe, rodzaje karnetów, ograniczenia oraz rzeczy do sprawdzenia. Nie dodawaj niepotwierdzonych atrakcji.
- **Nie sumuj** kilometrów podobszarów, jeżeli operator już podaje wspólny teren. Nie utożsamiaj tras przygotowanych z freeride, długości pojedynczego zjazdu z sumą tras ani dostępu do regionu z prawami podstawowego karnetu.
- Umieszczaj blok `Data odczytu / Źródło / Zakres` bezpośrednio pod tytułem zgodnie z [zasadami dat odczytu](../../../.github/zasady-dat-odczytu.md). Jeśli nie było ponownej weryfikacji, nie zmieniaj daty.
- Profil ośrodka może odsyłać do kraju i `porownania/`. Nie dodawaj linków zwrotnych z `kraje/` do planów w `wyjazdy/`.
- Po dodaniu miejsca zaktualizuj `kraje/README.md` i stronę kraju. Jeśli zmieniła się informacja wykorzystywana w porównaniu, zaktualizuj także odpowiednie `porownania/` zgodnie z [compare-resorts](../compare-resorts/SKILL.md). Nie twórz pustych katalogów.

## Kontrola jakości i publikacja

- Sprawdź, czy miejsce istnieje tylko raz, czy linki są poprawne i czy opisane liczby rzeczywiście odnoszą się do wskazanego ośrodka i karnetu.
- Sprawdź zgodność opisu z profilami sąsiednimi oraz brak ceny i terminów sezonowej oferty w uniwersalnym profilu ośrodka. Daty sezonu funkcjonowania samego terenu mogą występować jako dane operatora z podanym sezonem i źródłem.
- Sprawdź zgodność z [CONTRIBUTING.md](../../../.github/CONTRIBUTING.md), zasady dat odczytu i brak danych prywatnych.
- Przy zmianach plików stosuj [pull-request](../pull-request/SKILL.md); nie merguj bez polecenia. Raportuj wykonane kontrole i nierozstrzygnięte rozbieżności.
