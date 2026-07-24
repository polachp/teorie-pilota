# TODO

## 1. Komentovací nadstavba pro instruktory (příprava na revizi)

Cíl: instruktor si otevře stránku, u konkrétní sekce klepne na tlačítko a snadno pošle komentář/připomínku — bez znalosti GitHubu. Správce (admin) komentáře uvidí pohromadě a zapracuje.

Možnosti k rozhodnutí (zatím nerozhodnuto):

- [ ] **GitHub Issues s předvyplněním** — tlačítko „💬 Připomínka" u každé sekce otevře nové Issue s předvyplněným názvem předmětu/bodu. Zdarma, bez backendu; instruktoři potřebují GitHub účet.
- [ ] **Giscus/Utterances** (komentáře přes GitHub Discussions/Issues vložené pod stránku) — komentování přímo na webu; opět nutný GitHub účet.
- [ ] **Formulář bez přihlášení** (Google Forms / Formspree s polem „sekce") — nejnižší bariéra pro instruktory, admin dostává odpovědi do tabulky/mailu; o něco horší provázání s konkrétním místem textu.
- [ ] Vybrat řešení, implementovat tlačítko u sekcí, sepsat mini-návod pro instruktory.

## 2. Odborná revize textů (odloženo — čeká na tým instruktorů)

- [ ] Projít 34 míst označených `**⚠️ K verifikaci:**` a okolní texty:
  - [ ] Nouzové postupy (9) — hodnoty opadání, techniky vybírání režimů, záložní padák
  - [ ] Meteorologie (8) — číselné hodnoty, gradienty
  - [ ] Předpisy (5) — vše proti aktuálnímu znění předpisů
  - [ ] Nauka o létání (4) — mj. znění pětibodové kontroly dle praxe
  - [ ] Stavba a konstrukce PK (3) — lhůty prohlídek LAA
  - [ ] Letecká navigace (3) — doba letu vůči západu slunce, mapy
  - [ ] Zdravověda (2) — detaily dle Guidelines ERC
- [ ] Po dokončení revize odstranit sticky proužek z `_layouts/default.html`.

## 3. Detailní podstránky „K dalšímu studiu"

- [x] Hotové: všech 71 bodů má detailní podstránku (psáno řečí instruktora, klíčové pojmy tučně, terminologie ověřována z internetu — LAA, ŘLP/AIP, ERC, učebnice Vykouk aj.).
- [ ] Detaily obsahují **78 nových míst „⚠️ K verifikaci"** — přidat do odborné revize (sekce 2). Nejvíc: Předpisy 25, Nouzové postupy 16, Meteorologie 11.

## 4. Obrázky a schémata

- [ ] SVG ilustrace v paletě webu: rychlostní polára s režimy, profil křídla a úhel náběhu, části PK s popisky, rozdělení vzdušného prostoru.
- [ ] Složka `obrazky/`, vkládání `![popis](../obrazky/soubor.svg)`.

## 5. Testové otázky

- [ ] Získat reálné zkouškové okruhy/otázky (PDF od uživatele).
- [ ] Napojit na rozbalovací otázky v detailech, případně samostatná procvičovací stránka.

## Nápady k zvážení

- [ ] Vyhledávání v obsahu (lunr.js nebo jednoduché filtrování).
- [ ] Označení stavu sekce (ověřeno/v revizi) přímo u nadpisů.
- [ ] Tisková verze / PDF export pro žáky bez připojení.
