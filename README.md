# Teorie pro pilota padákového kluzáku

Web s teoretickými znalostmi ke kvalifikaci pilota PK, hostovaný na GitHub Pages: **https://polachp.github.io/teorie-pilota/**

## Struktura

```
index.md            # úvodní stránka s přehledem okruhů
teorie/*.md         # jeden soubor = jeden bod osnovy
_config.yml         # nastavení Jekyllu (titulek, vzhled)
```

## Jak přidat nový bod osnovy

1. Vytvoř soubor `teorie/<nazev-bodu>.md` (malá písmena, pomlčky místo mezer, bez diakritiky).
2. Piš obyčejný markdown — HTML se vygeneruje samo.
3. Přidej odkaz do seznamu v `index.md`: `[Název bodu](teorie/<nazev-bodu>.html)` (odkazuje se na `.html`, ne `.md`).

Po pushi do `main` se web během pár minut sám přegeneruje.
