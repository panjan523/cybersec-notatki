# Podstawy aplikacji

*Wygląd

Wygląd strony składa się z:
-Front endu

html - zbiór instrukcji co wyświetlac w przegladarce

css  - wygląd strony

java script - bardziej złożone i zaawansowane instrukcje.

-Back endu

baza - przechowywane są tutaj dane

infrastruktura - rzeczy które zaliczają sie do aplikacji internetowych jak urządzenia, serwery internetowe itd.

WAF ( web aplication firewall) - filtruje niebezpieczne pożadania

- Uniform Resource Locator (URL)

Url który pozwala na dostęp do różnej zawartości jak np. filmy czy strony.

http://user:password@abc.com:80/view-room?id=1#xyz

(http) Schemat - protokoł używany żeby uzyskac dostęp do strony

(user:password) Host/domena - NAJWAŻNIESZJA CZĘŚĆ. Mówi do której strony uzyskujesz dostęp.

:80 Port -  Służy do wskazania konkretnej aplikacji lub usługi

/view-room Scieżka - pokazuje podstronę na której jesteś

?id=1 Query String - zaczyna się pytajnikiem. przekazuje dodatkowe informacje do serwera internetowego.

#xyz Fragment - wskazuje na sekcje strony, kal przeskakiwanie to nagłowka lub tablicy.

- Wiadomości HTTP

Są to pakiety wymieniane między klientem a serwerem.

Dzieli się je na dwie kategorie:
Żądania - wysyłane przez użytkownika do serweru.

Odpowiedzi -  w drugą stronę.

Linia początkowa - mówi jaki rodzaj wiadomości został wysłany.

Nagłówki - podają dodatkowe informacje o HTTP

Pusta Linia - działa jako rozdzielacz

Struktura - miejsce w którym są przechowywane dane.

- Żądanie HTTP

Ścieżka URL - mówi serwerowi gdzie znaleść zasoby o które pyta użytkownk.

Wersja HTTP - mówi jaki protokoł został użyty do komunikacji między komputerem a klientem.

- Rodzaje nagłówków

Host - nazwa serweru gdzie wysyłane jest ządanie

User-Agent - informacje o przeglądarce

Referencja - url z ktorego wysylane jest zadanie

Ciasteczka 0- informacje które serwer wysyła przeglądarce do zachowania.

Rodzaj zawartosci - opisuje format zawartości.

- Status strony

Status strony jest zwracany trzyliczbową cyfrą oraz wyjaśnieniem statusu.

Status line - początek 

100-199 - serwer uzyskał część informacji i czeka na kolejne

200-299 - uzyskano wszystkie dane.

300-399 - dane zostaly przeslane do innej lokalizacji 

400-499 - błędy klienta

500-599 - błędy serwera

warto do nagłówka set-cookie dodawac httponly żeby nie były kradzione przez javascript lub secure do flagi żeby był tylko przesyłane przez https.

- Nagłówki zabezpieczające

Służą do wzmacniania zabezpieczeń strony.

W tym labolatorium przeglądnąłem podstawy struktur które budują strony internetowe. Rozbiłem URL na pojedyncze fragmenty żeby zrozumieć. Poznałem także struktury “nagłówków” które są fundamentami strony internetowej.