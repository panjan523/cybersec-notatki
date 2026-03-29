# Skanowanie luk

Luki sa miejscami które wymagają patchowania. Jest to proces łatania “dziur”

- Luki mogą prowadzić do masywnych uszkodzeń gdy nie są załatane

uwierzytelnione skany

- Podmiot hostu musi być podany do skanera luk
- Identyfikuje luki które mogą być użyte przez hakerów
- Podaje głębszą widoczność systemu poprzez skanowanie konfiguracji

nieuwierzytelnione skany

- Identyfikuje luki które mogą być przejęte przez zewnętrznego hakera który nie ma dostepu do podmiotu hostu

Wewnętrzne skany

Przeprowadzane ze srodka internetu

Skupia sie na lukach które mogą byc przejęte WEWNĄTRZ

Zewnetrzne skany 

- Przeprowadzane zewnętrznie od sieci
- Skupia sie na lukach które mogą byc przejęte ZEWNĄTRZ

CVE -Common Vulnerabilities and Exposures

Są to odpowiednie numeracje dla luk ktore zostały załatane. Jest to ogromna baza danych, każda luka ma inne unikalne oznaczenie.

CVVS  -  Common Vulnerability Scoring System.

- Są to oznaczenia w skali 0-10
- oznaczają poziom zagrożenia

![image.png](image%2023.png)

Labolatorium z openvas

W labolatorium miałem przeskanować dokument zrobiony za pomocą OpenVas. Jest to program, który skanuje adresy ip żeby zdobyć informację o zagrożeniach i ich skali cvvs. W przypadku tego labolatorium, luka miała najwyższą możliwą skale. OpenVas proponuje dla tej luki zmiany haseł.

![image.png](image%2024.png)