# Ogólne podstawy

Czym sie rozni MAC od IP?

Główna różnica polega na trwałości i zastosowaniu
adres MAC (fizyczny) jest unikalnym, niezmiennym identyfikatorem 
sprzętowym karty sieciowej, działającym lokalnie. Adres IP (logiczny) 
jest przypisywany tymczasowo przez sieć i służy do routingu danych w 
Internecie

ARP
to rodzaj wiadomości sieciowej, która umożliwia urządzeniom w sieci lokalnej 
(LAN) powiązanie logicznego adresu IP (warstwa 3 modelu OSI) z fizycznym
 adresem MAC (warstwa 2) karty sieciowej

DHCP

(Dynamic Host Configuration Protocol) to sieciowy protokół, który automatycznie przydziela urządzeniom (komputerom, 
telefonom, drukarkom) adresy IP oraz inne ustawienia sieciowe (maska, 
brama, DNS)

![image.png](image%208.png)

OSI 

jest to struktura złożona z 7 warstw która standaryzuje komunikację w sieciach komputerowych.

![image.png](image%209.png)

1. Fizyczna

Jest to przykładowo kabel ethernet

1. Data link

Odpowiada za konwersje. Dostaje dane z warstwy sieciowej i dostarcza do MACa.

1. Sieć
Podczas gdy niektóre protokoły w tej warstwie dokładnie określają, jaka 
jest "optymalna" ścieżka, którą dane powinny podążać, aby dotrzeć do 
urządzenia, powinniśmy wiedzieć o ich istnieniu tylko na tym etapie 
modułu sieciowego. Krótko mówiąc, protokoły te obejmują **OSPF** (**O**pen **S**hortest Path First) **i** RIP (Routing **Information** Protocol)
- Jaka ścieżka jest najkrótsza?
- Jaka ścieżka jest najbardziej wiarygodna?
- Która ścieżka ma szybsze połączenie fizyczne?
1. Transport

![image.png](image%2010.png)

1. Sesja

Po prawidłowym przetłumaczeniu lub sformatowaniu danych z warstwy prezentacji (warstwa 6), warstwa sesji (warstwa 5) rozpocznie tworzenie i utrzymywanie połączenia z innym komputerem, dla którego dane są przeznaczone. Po nawiązaniu połączenia tworzona jest sesja. Podczas gdy to połączenie jest aktywne, sesja również.

1. Prezentacja

Warstwa ta pełni rolę tłumacza danych do i z warstwy aplikacji (warstwa 7). Komputer odbierający zrozumie także dane przesłane do komputera w jednym formacie, przeznaczone w innym formacie. Na przykład, gdy wysyłasz wiadomość e-mail, drugi użytkownik może mieć dla Ciebie innego klienta poczty e-mail, ale treść wiadomości e-mail nadal będzie musiała być wyświetlana w ten sam sposób.

1. Aplikacja

Jest to najbardziej nam znana warstwa. Czyli to co nam się wyświetla na stronach internetowych.