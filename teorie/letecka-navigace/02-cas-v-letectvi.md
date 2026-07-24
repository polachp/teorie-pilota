[← Letecká navigace](../05-letecka-navigace.html#bod-2){: .drobecek}

# Používání času v letectví — UTC, SEČ, SELČ

*Detail k dalšímu studiu*

## Proč letectví potřebuje jednotný čas

Letadlo přeletí časové pásmo za pár desítek minut a letecké informace (zprávy o počasí, omezení prostorů) čtou piloti z mnoha zemí najednou. Kdyby každý dokument používal místní čas, byly by omyly na denním pořádku. Proto se v letectví celosvětově používá jediný čas:

**UTC (Coordinated Universal Time, koordinovaný světový čas)** — nástupce dřívějšího GMT, odvozený od atomových hodin a vztažený ke greenwichskému poledníku. V letecké frazeologii a zápisech se označuje písmenem **Z** („zulu"): zápis `1430Z` čteš „čtrnáct třicet zulu" = 14:30 UTC.

V UTC jsou uváděny: **AIP** (letecká informační příručka), **NOTAM** (zprávy o omezeních a změnách), meteorologické zprávy **METAR/TAF**, časy aktivace prostorů v AisView i tabulky východů a západů slunce.

## SEČ a SELČ — náš místní čas

- **SEČ (středoevropský čas)** = **UTC + 1 hodina**. Platí v zimní části roku.
- **SELČ (středoevropský letní čas)** = **UTC + 2 hodiny**. Platí zhruba od konce března do konce října (změna vždy o víkendu, posun o 1 h).

> Převod tam: **UTC → místní čas: přičti 1 h (SEČ) nebo 2 h (SELČ).**
> Převod zpět: **místní čas → UTC: odečti 1 h (SEČ) nebo 2 h (SELČ).**
> Příklad: 12:00 UTC = 13:00 SEČ = 14:00 SELČ.

Nejčastější chyba je špatný **směr** převodu. Pomůcka: v ČR je místní čas **vždy napřed** před UTC — když je v Greenwichi poledne, u nás už je po poledni.

## Praktické příklady z plánování letu

- **NOTAM:** „Prostor aktivován 0700–1500 UTC." V létě to znamená **9:00–17:00 SELČ** — kdo si neodečte dvě hodiny, klidně do prostoru vletí v domnění, že už je po aktivaci.
- **Západ slunce:** tabulka v AIP uvádí západ pro dané datum např. 1905 UTC — v létě je to **21:05 SELČ**.
- **Meteo:** METAR s časem `241100Z` je pozorování z 24. dne v měsíci, 11:00 UTC, tedy 13:00 SELČ.

## Na co si dát pozor

- **Přechod SEČ ↔ SELČ:** dvakrát ročně se posun mění. Zkontroluj, které období právě platí — hlavně na jaře a na podzim kolem změny času.
- **Aplikace a přístroje:** mobil ukazuje místní čas, letecké aplikace často UTC (nebo obojí). Vždy si ověř, na který čas se právě díváš.
- **Domluva s partou:** „sraz na kopci v 10" je místní čas, „prostor aktivní od 10" v NOTAMu je UTC. Při plánování přeletu si všechny časy převeď do jednoho systému.

## Otázky k procvičení

<details>
<summary>Kolik je 15:00 UTC v létě našeho místního času?</summary>
<p>17:00 SELČ — středoevropský letní čas je UTC + 2 hodiny.</p>
</details>

<details>
<summary>Co znamená písmeno Z za časovým údajem, např. 0900Z?</summary>
<p>Označení „zulu" — čas je uveden v UTC (koordinovaném světovém čase). 0900Z je tedy 9:00 UTC, v zimě 10:00 SEČ, v létě 11:00 SELČ.</p>
</details>

<details>
<summary>Proč se letecké dokumenty (NOTAM, METAR, AIP) uvádějí v UTC?</summary>
<p>Aby měly jednoznačný časový údaj nezávislý na časových pásmech a letním čase — piloti kdekoli na světě čtou stejný čas a nedochází k omylům při aktivaci prostorů nebo platnosti zpráv.</p>
</details>

[← Zpět na Leteckou navigaci](../05-letecka-navigace.html#bod-2){: .btn-zpet}
