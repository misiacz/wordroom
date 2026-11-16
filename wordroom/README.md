# Wordroom — Business English

Prosta aplikacja do nauki angielskiego słownictwa biznesowego z polskimi tłumaczeniami. Zawiera 296 haseł, definicje i przykłady.

## Funkcje

- Słownik z wyszukiwaniem po polsku i angielsku.
- Losowane fiszki ze znaczeniem i przykładem.
- Ćwiczenie pisowni z natychmiastowym sprawdzaniem.
- Quizy z wyborem odpowiedzi.
- Przycisk „Wygeneruj test”: 10 losowych haseł do wpisania po angielsku, wynik i poprawne odpowiedzi na końcu.
- Układ dopasowany do telefonów i komputerów.

## Uruchomienie

Otwórz `index.html` w przeglądarce. Możesz też uruchomić lokalny serwer w folderze projektu:

```sh
python3 -m http.server 8000
```

Następnie otwórz http://localhost:8000. Nie trzeba instalować zależności ani budować projektu.

## Dodanie do GitHub

1. Utwórz repozytorium na GitHub.
2. Rozpakuj paczkę i prześlij zawartość folderu `wordroom` do głównego katalogu repozytorium.
3. Zapisz pliki jako commit.

## Opcjonalne uruchomienie przez GitHub Pages

W ustawieniach repozytorium przejdź do **Settings → Pages**, wybierz **Deploy from a branch**, gałąź `main` i folder `/ (root)`, a następnie zapisz. Włączanie Pages może udostępnić stronę publicznie; dostępność zależy od ustawień i planu GitHub.

## Edycja słownictwa

Hasła znajdują się w tablicy `WORDS` na początku `app.js`. Każde ma unikalne `id`, angielskie hasło `en`, polskie znaczenie `pl`, definicję `def` i przykład `example`.

## Struktura

- `index.html` — struktura strony
- `style.css` — wygląd i układ responsywny
- `app.js` — słownictwo i logika ćwiczeń
- `icon.svg` — ikona strony

Aplikacja działa w przeglądarce. Nie wymaga kluczy API ani zaplecza serwerowego. Odpowiedzi z testu są przechowywane tylko w pamięci bieżącej sesji; odświeżenie strony rozpoczyna nowy test.
