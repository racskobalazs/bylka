# Bylka – nyilvános oldalak

A Bylka blokk- és számlaolvasó alkalmazás nyilvános dokumentumai. Ezeket a
Google Play Console-ba kell megadni (kötelező elemek), és a GitHub Pages
szolgálja ki őket.

| Oldal | URL |
| --- | --- |
| Adatkezelési nyilatkozat (magyar) | https://racskobalazs.github.io/bylka/privacy-hu.html |
| Privacy Policy (English) | https://racskobalazs.github.io/bylka/privacy-en.html |
| Fiók és adatok törlése | https://racskobalazs.github.io/bylka/fioktorles.html |
| Nyitólap | https://racskobalazs.github.io/bylka/ |

## Fióktörlés

A törlési oldal két utat kínál:

1. **Google-bejelentkezés** – a felhasználó a Google-fiókjával igazolja, hogy
   övé a fiók, és azonnal törölheti (e-mail-küldés nélkül is működik).
2. **E-mailes megerősítés** – a megadott címre küldött linkkel igazol, majd
   törli a fiókot.

Mindkét út a Supabase `delete-account` edge functiont hívja, amely a fiókot és
**minden** kapcsolódó adatot eltávolít (blokkok, feltöltött képek, keret,
jogosultság, AI-limit sorok).

Az alkalmazás forráskódja külön, privát repóban él.

## GitHub Pages

Beállítás: **Settings → Pages → Source: Deploy from a branch → `main` / `/` (root)**.
