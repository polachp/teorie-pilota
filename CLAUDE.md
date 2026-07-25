# CLAUDE.md

Tento soubor popisuje projekt pro práci s Claude Code (claude.ai/code) i pro lidské přispěvatele.

## Co to je

Studijní web **Teorie pro pilota padákového kluzáku** — teoretické znalosti ke kvalifikaci PILOT podle osnovy **LAA PL 3, Hlava 2** (bod 2.3). Dvojí účel: opora pro instruktora při přednáškách (tahák = nadpisy bodů) a studijní materiál pro žáky. Obsah i UI česky — drž se toho.

Web: https://polachp.github.io/teorie-pilota/

## Architektura

```
markdown (znalostní báze)  →  Jekyll (GitHub Pages)  →  statický web
```

- **Žádný build lokálně, žádný server.** HTML generuje GitHub Pages automaticky při pushi do `main` (theme Cayman + vlastní přepisy). Nasazení trvá ~1–2 minuty.
- Zdroj pravdy jsou výhradně `.md` soubory — HTML se nikam necommituje.

## Struktura

```
index.md                     # úvod: rozcestník předmětů (dlaždice), O projektu
teorie/NN-<predmet>.md       # 8 předmětů, přehledová vrstva („tahák")
teorie/<predmet>/NN-<bod>.md # detailní podstránky bodů („K dalšímu studiu")
dokumenty/PL3.pdf            # zdrojový předpis (odkaz z úvodu, nové okno)
_layouts/default.html        # šablona: klikací hlavička → úvod, revizní proužek
assets/css/style.scss        # téma „Letová hladina" (přepis Cayman + vlastní styly)
_config.yml                  # titulek, podtitulek, theme, lang: cs
TODO.md                      # roadmapa projektu (komentáře instruktorů, revize…)
```

**Stav obsahu:** kompletní — všech 71 bodů osnovy má výklad v přehledu i detailní podstránku. Texty jsou psány řečí instruktora s praxí, klíčové odborné pojmy tučně s definicí, terminologie ověřována proti českým zdrojům (LAA, ŘLP/AIP, ČHMÚ, ERC, učebnice Vykouk). Čeká se na odbornou revizi (viz TODO.md): ⚠️ K verifikaci je ~112 míst (34 v přehledech + 78 v detailech).

### Přehledová stránka předmětu

- H1 = název předmětu, pak řádek `**Rozsah výuky:** …` (hodinové dotace z PL 3, bod 2.2).
- Každý bod osnovy = H2 s kotvou: `## 1. Název bodu {#bod-1}`. **Nadpisy bodů = přesné znění osnovy PL 3, neměnit.**
- Pod bodem stručný výklad (odrážky s tučnými pojmy, poznámky „Prakticky:" / „Proč to pilota zajímá:", vzorce a poučky jako blockquote `> **…**`).
- Odkaz na detail: `[K dalšímu studiu →](<predmet>/NN-<bod>.html){: .btn-detail}`.
- Konec souboru: `[← Zpět na přehled](../index.html){: .btn-zpet}`.

### Detailní podstránka bodu

- První řádek drobeček: `[← <Předmět>](../NN-<predmet>.html#bod-N){: .drobecek}` — vrací ke kotvě nadřazené sekce.
- Pak H1, řádek `*Detail k dalšímu studiu*`, rozšířený výklad, sekce `## Otázky k procvičení` s rozbalovacími `<details><summary>otázka</summary><p>odpověď</p></details>`.
- Konec: `[← Zpět na <Předmět>](../NN-<predmet>.html#bod-N){: .btn-zpet}`.

## Konvence

- **⚠️ K verifikaci:** nejistá tvrzení se značí samostatným řádkem `**⚠️ K verifikaci:** <co ověřit>`. Odstraňuje se až po odborné revizi instruktorem. Nikdy nevymýšlet čísla paragrafů ani konkrétní hodnoty bez označení.
- **Barvy:** oranžová/zlatá `#F0A63C` = navigace (drobeček, K dalšímu studiu, spodní Zpět, revizní proužek); modrá = obsah (nadpisy, dlaždice, odkazy). Paleta: navy `#0E2A4E`, letová modrá `#1E7BC4`, ocelová `#114B77`, mlžná `#F2F8FD`.
- **Typografie:** Barlow Condensed (nadpisy), Barlow (text), Google Fonts. Velikosti písma jen v hodnotách vycházejících na celé px (16/15/13/18/22/24/28/36) — ostrost na mobilech.
- **Mobile-first:** dotykové cíle min. 44–48 px, klikatelné celé plochy, rádius tlačítek 10 px (hranatější, ne pilulky).
- Revizní proužek (sticky) je v `_layouts/default.html` — po dokončení odborné revize smazat jeden `<div class="revize">`.

## Workflow

1. Uprav `.md` → commit → `git push origin main`.
2. Ověření = počkat na přegenerování GitHub Pages a zkontrolovat na mobilu.
3. Hromadné psaní obsahu: paralelní subagenti po předmětech, každý upravuje právě jen své soubory (vlastní složka detailů + vlastní přehled), git dělá orchestrátor. Vždy vyžadovat značení „⚠️ K verifikaci". Po doběhnutí strukturální kontrola skriptem (drobečky, kotvy, počty otázek, existence cílů odkazů), pak jeden commit.

## Odborná revize (probíhá)

- Uživatel (instruktor) diktuje správné znění — jeho formulace mají **přednost před textem vygenerovaným AI i před literaturou** (příklad: klasifikace odporu = 4 části: třecí, tvarový, interferenční, indukovaný; pojem „škodlivý odpor" se nepoužívá).
- Korekci vždy promítnout do **obou vrstev** (přehled + detail) včetně kontrolních otázek a navazujících zmínek jinde na webu (ověřit grepem), pak odstranit příslušný řádek „⚠️ K verifikaci".
- Sticky revizní proužek v `_layouts/default.html` se odstraní až po dokončení celé revize.
