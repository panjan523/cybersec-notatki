# JavaScript w przeglądarce - podstawy

Javascript pozwala deweloperom internetowym dodawanie interaktywnych rzeczy na stronę na przykład animacje. Jest o język INTERPRETOWANY czyli kod jest czytany linijka po linijce i wykonywany w czasie rzeczywistym.

- Zmienne

pozwalają na zachowywanie w nich danych.

przykłady:

string - tekst,

number,

boolean - prawda lub fałsz.

- Funkcje

Jest to blok kodu który służy do wykonania pewnego zadania.

- Pętle

Mają zastosowanie tak długo aż status jest na “true”.

- Wgląd na JS

W Chrome za pomocą skrótu CTRL + Shift + I można otworzyć konsolę lub inspect.

External Javascript (zewnetrzny) to sposób przechowywania kodu w osobnym pliku z rozszerzeniem js.

Internal (wewnętrzny) natomiast daje kod bezpośrednio w dokumencie html.

W javie można dodawać powiadomienia z którymi użytkownik może wchodzić w interakcję. Zaliczamy do nich:

Alert

Pozwala na pokazanie powiadomienia w przeglądarce. Można ją aktywować wpisując przykładowo: alert(”abc”).

Prompt

Podobny do alert natomiast użytkownik może wprowadzać dane.

Confirm 

Bardzo podobny do alert natomiast posiada dodatkowy przycisk cancel. użytkownik może zatwierdzić albo anulować akcje.

Przykładowo w ten sposób hakerzy mogą przeszkadzać w użytkowani strony: 

 `<!DOCTYPE html>
<html lang="en">
<head>
    <title>Hacked</title>
</head>
<body>
    <script>
        for (let i = 0; i < 500; i++) {
            alert("Hacked");
        }
    </script>
</body>
</html>`

Podany wyżej kod powtarza 500 razy powiadomienie “Hacked”.

- Control flow

Jest to uporządkowany sposób w jaki warunki są spełniane w programie.

- Minifikacja

Jest to proces w którym plik jest przekształcany tak żeby nie był zdatny do przeczytania przez człowieka. Redukuje to rozmiar pliku i przyspiesza działanie.

przykładowo można użyć tej strony do zaciemnienia kodu

[https://codebeautify.org/javascript-obfuscator](https://codebeautify.org/javascript-obfuscator)

![image.png](image%2011.png)

Jest to nadal funkcjonujący kod.

Ten sam kod można rozkodować używając podobnych stron.

NIGDY nie powinno się dawać wrażliwych danych do kodu JS, ponieważ użytkownik w kodzie źródłowym bez problemu może znaleźć dane.

- Podsumowanie

W tym laboratorium prześledziłem podstawowe funkcje działania kodu w JavaScript. Poznałem jak działają zmienne, funkcje, powiadomienia i działanie JavaScriptu, który przykładowo w porównaniu do języka C nie jest językiem kompilowanym tylko interpretowanym. Bardzo ważne jest żeby pamiętać o tym żeby nie dawać wrażliwych danych do kodu JS. Aby ulepszyć działanie kodu można go zmimifikować.