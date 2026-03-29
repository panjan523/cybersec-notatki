# JohnTheReaper

Działanie

- `john [options] [file path]`

Przydatny program

```bash
 wget https://gitlab.com/kalilinux/packages/hash-identifier/-/raw/kali/master/hash-id.py
$ python3 hash-id.py

```

Umożliwia rozpoznanie typu Hasha.

![image.png](image%2025.png)

W podanym przykładzie miałem z hasha w pliku “hash1.txt” rozpoznać jaki to jest typ hasha. Na powyższym przykładzie za pomocą funkcji cat odczytałem hash , a następnie go zidentyfikowałem programem hash-id.py.

Później podaną wartość musiałem rozkodować encryptorem.

![image.png](image%2026.png)

![image.png](image%2027.png)

![image.png](image%2028.png)

![image.png](image%2029.png)

Podobnym schematem rozkodowałem resztę hashy, następująco było MD5, Sha1, Sha256, whirlpool.

**NTHash** 

- jest to format stosowany w Windowsie, zawiera informację o użytkowniku i hasłach.

Z jakiegoś powodu usunął mi się terminal po odświeżeniu maszyny wirtualnej, i później nie mogłem zobaczyć ponownie hasła. Pojawiło się tylko za pierwszym razem gdy użyłem komendy “john —format:nt ntlm.txt”.  Użyłem tych komend:

![image.png](image%2030.png)

Hasło które wyszło to: “mushroom”

/etc/shadow/

- Jest to katalog w linuxie, który przechowywuje hashe haseł.

![image.png](image%2031.png)

Hasło to było 1234

Single crack mode 

Jest to tryb w którym JohnTheReaper szybciej sprawdza hasła, bazujac na tym że jest na podstawie nazwy użytkownika. Np. dla nazwy ‘Marcus’ może to być: Marcus1, Marcus2, Marcus3 itd.

![image.png](image%2032.png)

![image.png](image%2033.png)

Do single cracka należy wcześniej zedytować plik jak w zdjęciu pierwszym. Należy dopisać nazwę użytkownika i po niej dwukropek. Później użyć komendy jak na drugim zdjęciu.

Sprawdziłem tez wczesniej jaki jest typ hasha 

![image.png](image%2034.png)

Crackowanie Zipów

![image.png](image%2035.png)

![image.png](image%2036.png)

Do crackowania zipów służy zip2john. Na poczatku zip trzeba przekształcić na hash który john bedzie mógł odczytać. Pózniej trzeba zcrackowac hasło komenda na zdjęciu. Podane hasło to pass123.

Crackowanie RAR

Jest analogiczne do zipów. Różnica jest taka że uzywa się rar2john

![image.png](image%2037.png)

![image.png](image%2038.png)

miedzy otwieraniem zipa a rar jest taka różnica, że przy rar trzeba dodac odpowiedni przyrostek zeby wybrac gdzie rozpakowac. W tym przypadku ‘e’ rozpakowywuje w sciezce ktorej jest user.

SSH

W przypadku do rar i zipa jest drobrna różnica. Trzeba użyć skryptu z pythona.

![image.png](image%2039.png)