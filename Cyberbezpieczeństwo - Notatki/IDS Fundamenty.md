# IDS Fundamenty

(Intrusion Detection System)

Firewall sprawdza połączenie i je odrzuca gdy złamie jego zasady.

Żeby go usprawnić możemy użyć IDS. Jest to program do sprawdzania aktywności połączenia.

Jeśli haker pomyślnie złamie firewalla, to IDS sprawdza aktywniść.

Działa podobnie na zasadzie kmaery w budynku. Może przykładowo zarejestrować intruza jak włamuje się do budynku.

IDS dzielimy na dwie kategorie: 

![image.png](image%2020.png)

HIDS: 

- jest zainstalowany na hoście
- pokazuje szczegółowo aktywność hosta i wyłącznie tyle

NIDS 

- Wykrywa zagrożenia w całej sieci, niezależnie od hosta.

SNORT

- Pozwala na detekcję wirusów. Można ustawiać mu własne zasady

Packet sniffer mode 

- czyta i wyświetla pakiety sieci bez analizowania ich (czasem trzeba przeczytać pakiety bez ingerencji w nie)

Packet logging mode 

- Sprawdza sieć w czasie rzeczywistym, pokazuje alerty w konsoli dla administratorów.

Network Intrusion Detection System mode

- Monitoruje sieć w czasie rzeczywistym i używa stworzonych reguł. Gdy atak spełnia wymogi zasady, uruchamia się alert.

`alert icmp any any -> 127.0.0.1 any (msg:"Loopback Ping Detected";
sid:10003; rev:1;)`

Udało mi się połaczyć i otrzymać ping o tym że informacja została odebrana.  Po próbie połaczenia wyświetla się informacja “Ping Detected”. Adres który probował się połaczyć to 10.11.90,211

![image.png](image%2021.png)

![image.png](image%2022.png)