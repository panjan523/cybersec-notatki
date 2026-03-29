# Burp Suite

FoxyProxy działa jak znak drogowy. Zamiast przesyłać do interneru, dane trafiają do burpa gdzie są kontrolowane.

Intercept w burpie działa na zasadzie policjanta. Gdy jest wyłączony to dane nie sa kontrolowane. Natomiast gdy jest włączony to każdy pojedynczy ruch jest kontrolowany przez burpa. Wtedy ma się pełną kontrolę nad tym co trafia na serwer. 

![image.png](image%2014.png)

W tym laboratorium udało mi się uchwycić flagę w aplikacji Burp. Osiągnąłem to poprzez przeszukiwanie w stronie podstron w której jedna z nich posiadała flagę. Zapoznałem się także z interfejsem Burpa i przede wszystkim jego najważniejszą zakładką: Proxy. Żeby program działał prawidłowo, musiałem z pomocą wtyczki foxyproxy stworzyc protokół proxy, żeby istniała komunikacja.

Dodanie do zakładki “scope” powoduje, że wychwytywane są tylko strony z podanego linku. Nie są pobierane wszystkie strony co może obciązać RAM.