# Technologie Obiektowe 2 - Bus Registration App

## Opis

Aplikacja ma na celu wspomagać pracę firmie przewozowej. Firma posiada
flotę autobusów i przewozi pasażerów z miasta A do miasta B.

## Wymagania

* możliwość rezerwacji przejazdów przez klientów,
* możliwość zarządzania przejazdami przez firmę (dodawanie, usuwanie przejazdów)

## Założenia projektu

### Założenia dla pasażera

* w celu możliwości rezerwacji przejazdu pasażer musi być zarejestrowany
* pasażer może zarezerwować wiele przejazdów, ale przejazdy nie mogą sie nakładać
i muszą być w określonym odstępie czasowym
* pasażer nie może zarezerwować przejazdu jeżeli czas do odjazdu jest krótszy niż godzina
* pasażer nie może zrezygnować z przejazdu ze zwrotem pieniędzy jeśli czas do odjazdu
jest krótszy niż godzina
* potwierdzenie rejestracji przejazdu jest wysyłane na adres e-mail

### Założenia dla firmy przewozowej

* firma przewozowa ma prawa administratora do aplikacji
* firma ma możliwość dodania przejazdów różnych typów 
np. przejazd okresowy, przejazd jednorazowy, przejazd zastępczy, 
przejazd awaryjny,
* firma ma możliwość przeprowadzania operacji CRUD na przejazdach,
* możliwość dodania powiadomień lub alertów wysyłanych na e-mail do pasażerów
danego przejazdu, lub alertów ogólnych

## Wykorzystywane narzędzia

Program napisany jest w języku Java z wykorzystaniem następujących narzędzi:

* **Gradle** - jako narzędzie do budowania projektu i zarządzania bibliotekami
* **framework Spring** - w celu ułatwienia pisania aplikacji webowej i zastosowania wzorca MVC
* **Thymeleaf template engine** - do stworzenia GUI, wsparcie ze strony frameworka Spring ułatwia 
stworzenie szaty graficznej dla aplikacji
* **baza danych MySQL** - warstwa persystencji dla aplikacji
* **JUnit i Spock test framework** - do testowania aplikacji