# Hydra

W skrócie jest to program do złamywania haseł

W tym labolatorium udało mi się złamać dwa hasła za pomocą hydry. 

-l   odpowiada za nazwe lub login użytkownika

-P pobiera liste haseł

-t  ilość haseł uzywanych w tym samym momencie

 

![image.png](image%2015.png)

używając schematu komendy:

`hydra -l <username> -P <wordlist> MACHINE_IP 
http-post-form "/:username=^USER^&password=^PASS^:F=incorrect" -s 
<port> -V`

udało mi się złapać flagę do pierwszej części zadania.

W drugiej części analogicznie miałem znaleść hasło do shh. 

![image.png](image%2016.png)

Po znalezieniu hasła trzeba było się zalogować poprzez shh, a tam później była flaga u zdalnego użytkownika.