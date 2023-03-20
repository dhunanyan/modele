# MM - MiracleMash

**_MiracleMash_** jest to sklep internetowy (tzw: E-commerce) na którym można kupić/sprzedać różne produkty

---

## Zakup

### Scenariusze

- Uzytkownik wybiera produkty które chce kupic
- Pojawiają się one w koszyku
- Uzytkownik przechodzi do kasy, zatwierdzając prudkty w koszyku
- System liczy sumę cen wszystkich produktów zawartych w koszyku
- System sprawdza stan konta uzytkownika zwracając mu róznicę jego salda i łącznej sumy produktów
- System sprawdza czy otrzymana liczba jest liczbą ujemną czy dodatnią
- Jeśli jest to liczba ujemna, to:
  - Mozliwośc zatwierdzenia zakupu jest zablokowana i wyświetlany jest komunikat o niewystarczającyh środków na koncie wraz z molzliwością doładowania.
  - Uzytkownik nie doładowuje konta i opuszcza kasę:
    - Zakup nie zostaję sfinalizowany
    - Uzytkownik jest na stronie głównej, gdzie moze kontynuowac wybór produktów, przy czym wcześniej wybrane ma w koszyku.
  - Uzytkownik nie doładowuje konta, ale nie opuszcza kasy:
    - Sesja uzytkownika gaśnie po 5 minutach
    - Zakup nie zostaję sfinalizowany
    - Potrzebne jest ponowne logowanie
  - Uzytkownik wybiera opcję doładowania konta:
    - System przekierowuje uzytkownika do sekcji wyboru formy płatności
    - Uzytkownik wybiera blik
      - System przekierowuje uzytkownika do sekcji z pustym polem wpisania kodu blik
      - Uzytkownik wpisuje poprawny kod za pierwszym razem
        - Przychodzi

## Wyszukiwarka

Wyszukiwarka - dzięki niej użytkownik może szybko znaleźć interesującą go rzecz.

### Podstawowe Funkcjonalności:

- Wyświetlanie produktów z wyszukiwanymi parametrami

- Wyszukiwarce wyświetlają się produkty o zbliżonych parametrach, od najbardziej to najmniej trafnych.

- Wyszukiwanie synonimów lub autouzupełnianie.

- Inteligentne rozwiązania takie jak korekta błędów

- Wyświetlanie komunikatu z przekroju **„nie znaleziono towarów dla Twojego zapytania”**, w przypdaku braku wystąpienia w asortymencie konkretnego produktu lub produktu o zbliżonych parametrach,

- Możliwość sortowania i filtrowania wyników wyszukiwania.
