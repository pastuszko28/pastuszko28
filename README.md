# Wizytówka — repozytorium

Prosty szablon strony-wizytówki (jedna strona), gotowy do hostowania na GitHub Pages.

Co zawiera:
- `index.html` — strona główna
- `styles.css` — styl
- `avatar.jpg` — (opcjonalnie) Twoje zdjęcie / avatar
- `README.md` — ten plik

Jak spersonalizować:
1. Zmień w `index.html`:
   - tytuł (`<title>`) i nagłówek (`.name`)
   - opis (`.role`, `.about`)
   - linki w sekcji `links` (GitHub, LinkedIn, itp.)
2. Wstaw swoje zdjęcie jako `avatar.jpg` (lub zmień nazwę w HTML).
3. Możesz dostosować kolory w `styles.css` (zmienne CSS na górze).

Jak uruchomić lokalnie:
```bash
# otwórz plik index.html w przeglądarce:
# np. w VSCode: Live Server, lub:
python -m http.server 8000
# potem odwiedź http://localhost:8000
```

Jak wypchnąć na GitHub i uruchomić Pages:
1. Utwórz repo na GitHub (np. `wizytowka`).
2. W katalogu projektu:
```bash
git init
git add .
git commit -m "Initial: wizytówka"
git branch -M main
git remote add origin https://github.com/<twoj-login>/wizytowka.git
git push -u origin main
```
3. W ustawieniach repo (Settings → Pages) wybierz branch `main` i folder `/ (root)` oraz zapisz. Strona pojawi się pod:
`https://<twoj-login>.github.io/wizytowka/` (po kilku minutach)

Alternatywa: użyj `gh` CLI:
```bash
gh repo create <twoj-login>/wizytowka --public --source=. --remote=origin --push
```

Gotowe! Jeśli chcesz, mogę:
- wygenerować i wypchnąć pliki za Ciebie (poproszę dostęp / uprawnienia lub polecenia),
- dodać prosty workflow CI/CD do automatycznego deployu,
- spersonalizować wygląd (kolory, układ) według Twoich preferencji.
