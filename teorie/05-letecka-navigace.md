# Letecká navigace

**Rozsah výuky:** bez kvalifikací 1,0 h · s kvalifikací PPG/MPG 0,5 h · ostatní piloti 0,25 h

## 1. Tvar zeměkoule, rovnoběžky a poledníky

Země není přesná koule, ale **geoid** — na pólech zploštělé těleso; pro navigaci ji nahrazujeme referenčním elipsoidem (GPS používá **WGS-84**). Na povrchu je položena souřadnicová síť:

- **Poledníky (meridiány)** — půlkružnice spojující severní a jižní pól. Základní (nultý) poledník prochází Greenwichem; od něj měříme **zeměpisnou délku** 0–180° východně (E) nebo západně (W).
- **Rovnoběžky** — kružnice rovnoběžné s rovníkem. Od rovníku měříme **zeměpisnou šířku** 0–90° severně (N) nebo jižně (S). Rovník je nejdelší rovnoběžka, k pólům se zkracují.
- **Zeměpisné souřadnice** = šířka + délka, udávané ve stupních, minutách a vteřinách (1° = 60′). ČR leží zhruba na **50° N, 15° E**.

**Prakticky:** 1 minuta zeměpisné šířky odpovídá 1 námořní míli (1 852 m) — na poledníku vždy, na rovnoběžce jen na rovníku. Souřadnice jsou jednoznačný způsob, jak nahlásit polohu (např. záchranné službě).

## 2. Používání času v letectví — UTC, SEČ, SELČ

V letectví se celosvětově používá **UTC** (koordinovaný světový čas, dříve GMT, v letecké frazeologii „zulu", značka Z). Všechny letecké dokumenty — AIP, NOTAM, meteorologické zprávy, časy východu a západu slunce — jsou uváděny v UTC, aby nedocházelo k omylům mezi časovými pásmy.

> **SEČ (středoevropský čas) = UTC + 1 h**
> **SELČ (středoevropský letní čas) = UTC + 2 h**
> Převod: 12:00 UTC = 13:00 SEČ = 14:00 SELČ. Naopak: z místního času odečti 1 h (v zimě) nebo 2 h (v létě).

**Proč to pilota zajímá:** kdo si při čtení NOTAMu nebo METARu splete UTC s místním časem, může se ocitnout v prostoru v době jeho aktivace nebo létat po západu slunce.

## 3. Východ a západ slunce — posun v ročních obdobích

Časy východu a západu slunce se během roku výrazně mění — je to důsledek sklonu zemské osy:

- **Letní slunovrat (cca 21. 6.)** — nejdelší den, v ČR slunce vychází kolem 5. hodiny a zapadá kolem 21. hodiny místního času.
- **Zimní slunovrat (cca 21. 12.)** — nejkratší den, východ kolem 8. a západ kolem 16. hodiny.
- **Rovnodennosti (březen, září)** — den i noc přibližně 12 h.

**Proč to pilota zajímá:** lety padákovým kluzákem se provádějí **ve dne, podle pravidel letu za viditelnosti (VFR)** — použitelná letová doba se tedy s ročním obdobím zásadně mění. Přesné časy pro dané místo a den zjistíš v AIP ČR nebo z běžných tabulek/aplikací; plánuj přistání s rezervou před západem slunce, protože osvětlení a termické podmínky se v podvečer rychle mění.

**⚠️ K verifikaci:** přesné vymezení povolené doby letu (den = od východu do západu slunce, případně občanský soumrak ±30 min) podle aktuálního znění předpisů pro SLZ (ZL-1/pravidla létání) — uvést přesnou citaci.

## 4. Mapy — zobrazení, měřítka, topografická situace

Mapa je zmenšené rovinné zobrazení zemského povrchu. Základem pro VFR létání v ČR je **letecká mapa ICAO ČR v měřítku 1 : 500 000** — 1 cm na mapě odpovídá 5 km ve skutečnosti.

- **Měřítko** — poměr vzdálenosti na mapě ke skutečnosti; čím menší číslo za jedničkou, tím podrobnější mapa.
- **Topografická situace** — mapa zobrazuje terén (vrstevnice, barevná hypsometrie — čím hnědší, tím vyšší), vodstvo, sídla, silnice, železnice, lesy a **kóty** významných vrcholů.
- **Letecký obsah** — řízené a omezené prostory (CTR, TMA, prostory P/R/D), letiště, překážky (vysílače, dráty lanovek). Výšky a nadmořské výšky jsou na mapě ICAO uváděny ve stopách (ft).

**Prakticky:** i pilot PK musí umět z mapy vyčíst, zda jeho startoviště a plánovaná trať nezasahují do řízeného či zakázaného prostoru. Mapa se pravidelně aktualizuje — létej s platným vydáním (dnes typicky v digitální podobě v mobilní aplikaci).

**⚠️ K verifikaci:** aktuální oficiální zdroj mapy ICAO ČR (vydává ŘLP ČR / AIM) a zda jsou výšky na české mapě ICAO skutečně ve ft.

## 5. GPS — princip, zobrazení, použití

**Princip:** přijímač GPS měří čas šíření signálu z družic obíhajících Zemi; ze vzdáleností k **nejméně čtyřem družicím** vypočte svou polohu (šířka, délka, výška). GPS je pasivní — přijímač nic nevysílá.

**Co pilotovi ukazuje:**

- **polohu** a záznam tratě (tracklog — dnes standard pro soutěže i vlastní rozbor letu),
- **rychlost vůči zemi (groundspeed)** — porovnáním s rychlostí vůči vzduchu lze odhadnout vítr,
- **směr letu vůči zemi** a navigaci k zadanému bodu (vzdálenost, kurz),
- **GPS výšku** — geometrickou výšku nad elipsoidem WGS-84.

> **GPS výška ≠ barometrická výška.** GPS měří geometricky (chyba typicky v jednotkách až desítkách metrů, nezávisí na počasí), výškoměr měří tlak (přesnější krátkodobě, ale závisí na nastavení a změnách tlaku). Pro srovnávání s výškami prostorů je rozhodující **barometrická** výška.

**Prakticky:** GPS je pomocník, ne náhrada navigace — baterie se vybíjí, signál může vypadnout. Základem zůstává mapa a srovnávací navigace.

## 6. Srovnávací navigace

Základní navigační metoda VFR létání: **průběžné porovnávání mapy se skutečným terénem** pod sebou. Pilot si drží orientaci podle výrazných **orientačních bodů**:

- **liniové** — řeky, silnice, železnice, elektrovody, okraje pohoří (dobře se podle nich „vede" trať),
- **plošné** — města, vodní plochy, letiště, velké lesní celky,
- **bodové** — vysílače, kostely, hrady, komíny, křižovatky.

**Postup:** před letem si trať projdi na mapě a vyber si kontrolní body; za letu postupuj **od mapy k terénu** (vím, co mám vidět, a hledám to), při ztrátě orientace naopak od terénu k mapě. Mapu drž zorientovanou po směru letu.

**Prakticky:** u přeletů na PK je srovnávací navigace hlavním nástrojem, jak se nedostat do řízeného prostoru a jak včas vybrat vhodné přistávací plochy podél trati.

## 7. Postup pro nastavování výškoměru

Barometrický výškoměr měří tlak vzduchu a převádí ho na výšku — ukazuje ale správně jen tehdy, je-li správně **nastaven na referenční hladinu**:

- **QNH** — výškoměr ukazuje **nadmořskou výšku** (výšku nad střední hladinou moře). Nastavení vhodné pro srovnávání s kótami na mapě a s výškovými hranicemi prostorů.
- **QFE** — výškoměr ukazuje **výšku nad zvoleným místem** (typicky nad startovištěm nebo přistávací plochou); na tomto místě ukazuje nulu.

**Postup na startovišti:** znáš-li **nadmořskou výšku startoviště** (z mapy, z kóty), nastav výškoměr tak, aby ji ukazoval — tím máš nastaveno QNH bez znalosti aktuálního tlaku. Chceš-li QFE, vynuluj výškoměr na místě startu.

**Prakticky:** tlak se během dne mění, proto výškoměr před každým letem znovu srovnej. Pamatuj, s čím letíš — údaj „500 m" znamená při QNH nadmořskou výšku, při QFE výšku nad startovištěm; záměna vede k chybnému odhadu výšky nad terénem i vůči prostorům.

**⚠️ K verifikaci:** přesné definice Q-kódů (QNH/QFE/QNE) dle platné letecké terminologie a zda je pro SLZ v ČR předepsáno konkrétní standardní nastavení.

[← Zpět na přehled](../index.html){: .btn-zpet}
