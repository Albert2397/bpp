# Broń Palna Polska — statyczna kopia

Serwis jest zbudowany z klasycznych plików HTML i CSS. Nie wymaga systemu CMS ani procesu kompilacji.

## Struktura

- `index.html`, `blog.html` — strona główna i indeks wpisów.
- `pages/` — podstrony działów, kontakt, o nas, testy i polityka prywatności.
- `articles/` — pełne lokalne kopie artykułów z WordPressa.
- `assets/css/` — arkusz stylów.
- `assets/images/` — obrazy pobrane z artykułów.
- `sitemap.xml`, `robots.txt` — pliki SEO.

Aby sprawdzić stronę lokalnie, uruchom z tego katalogu prosty serwer HTTP, np. `python3 -m http.server 8000`, a następnie otwórz `http://localhost:8000`.

## Osadzenie aplikacji testowej

W `pages/testy.html` znajduje się iframe jako placeholder. Ustaw jego atrybut `src` na publiczny adres aplikacji testowej, aby wyświetlać ją na stronie.

## Globalny font

Font dla wszystkich stron jest skonfigurowany w `assets/css/styles.css`: `@import` pobiera go z Google Fonts, a zmienna `--font-family` ustawia rodzinę i fonty zastępcze. Przy zmianie fontu zaktualizuj oba wpisy w tym pliku. Nowe strony powinny dołączać ten arkusz stylów; nie wymagają osobnych linków do Google Fonts.
