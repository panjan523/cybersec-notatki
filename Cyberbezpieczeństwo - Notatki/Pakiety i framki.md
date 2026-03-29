# Pakiety i framki

Pakiet - jest to kawałek informacji z warstwy 3. Zawiera informacje o tym jak adres Ip. Są wydajną opcją komunikacji. Dane są wymieniane  małych kawałkach przez to jest mniejsze szansa na obciążenia podzespołów.

Ramka - jest używana w warstwie drugiej (data link). Dodaje dodatkowe informacje takie jak adres MAC. 

TCP - Transmission Protocol System.

jest zawart w warstwach:

- aplikacji
- transportowej
- internetowej
- interfejsu sieciowego

TCP zawiera pewne nagłówki:

![image.png](image%2017.png)

Three-way handshake

- Jest to podstawowy proces w protokole TCP, służący do nawiązania niezawodnego połączenia między klientem a serwerem przed przesłaniem właściwych danych

SYN - klient inicjuje połączenie

SYN-ACK - odbieranie żądanie. ACK potwierdza odbiór i wysyła własną flagę SYN.

ACK - Klient odbiera SYN-ACL i odsyła ostateczny pakiet do ACK. W tym momencie połączenie jest ustawione.

![image.png](image%2018.png)

UDP (User Datagram Protocol) 

- jest to protokół który nie wymaga stałego połączenia między dwoma urządzeniami. Dla przykładu uzgadnianie trój-etapowe nie zadziała gdy nie ma synchronizacji między dwoma urządzeniami.
- jest szybszy nic TCP natomiast UDP nie obchodzi czy dostanie dane czy nie.

Nagłówki UDP:

![image.png](image%2019.png)

Port - jest to unikalna pstać. Urządzenia sieciowe używają portów do egzekwowania surowych zasad podczas komunikowania się ze sobą.

Porty są w przedziale od 0-65535.