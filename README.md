# Suzy Style — Cenovnik

Statički cenovnik za šminkanje, optimizovan za mobilne telefone i QR kod.

## Lokalno pregledanje

```bash
cd cenovnik
python3 -m http.server 8080
```

Otvori: http://localhost:8080

## Besplatan hosting (GitHub Pages)

### Prvi put (jednokratno)

1. Na [github.com](https://github.com) → **New repository**
2. Ime repoa: npr. `suzy-style-cenovnik` (Public)
3. **Ne** štikliraj "Add a README" — repozitorijum treba da bude prazan
4. U terminalu u folderu `cenovnik`:

```bash
git remote add origin https://github.com/TVOJ-USERNAME/suzy-style-cenovnik.git
git push -u origin main
```

5. Na GitHub-u: **Settings → Pages**
6. **Build and deployment → Branch:** `main`, folder `/ (root)` → **Save**
7. Za 1–2 min sajt je na: `https://TVOJ-USERNAME.github.io/suzy-style-cenovnik/`

Taj link stavi u QR kod.

### Kasnije izmene (cene, telefon, Instagram)

**Opcija A — na GitHub-u (najlakše):**
1. Otvori repozitorijum → `index.html` → ikonica olovke (**Edit**)
2. Promeni cenu ili tekst → **Commit changes**
3. Sajt se osveži za ~1 minut

**Opcija B — iz Cursora:**
1. Izmeni `index.html` lokalno
2. U terminalu:

```bash
cd cenovnik
git add index.html
git commit -m "Ažurirane cene"
git push
```

## Izmena cena

Uredi `index.html` — sekcije sa klasom `price-list`. Svaka stavka ima naziv usluge i cenu.

## Fajlovi

- `index.html` — glavna stranica
- `style.css` — stilovi (zlatno-crna tema)
- `assets/logo.webp` — logo iz zipa
- `assets/favicon.png` — ikonica u tabu
