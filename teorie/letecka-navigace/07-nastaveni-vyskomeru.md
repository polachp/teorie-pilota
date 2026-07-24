[← Letecká navigace](../05-letecka-navigace.html#bod-7){: .drobecek}

# Postup pro nastavování výškoměru

*Detail k dalšímu studiu*

## Princip: výškoměr je tlakoměr

Barometrický výškoměr měří **statický tlak vzduchu** a převádí ho na výšku podle standardní atmosféry (pokles zhruba **1 hPa na 8 m** v nižších hladinách). Z toho plyne zásadní věc: výškoměr neukazuje „výšku", ale **výšku nad zvolenou tlakovou hladinou**. Jaká hladina to je, určuješ ty svým nastavením — a proto musíš vždy vědět, **na co máš nastaveno**.

## QNH — nadmořská výška

**QNH** je tlak přepočtený na střední hladinu moře (podle standardní atmosféry). Výškoměr nastavený na QNH ukazuje **nadmořskou výšku** (altitude, výšku nad mořem):

- na startovišti ukazuje **nadmořskou výšku startoviště** (kótu),
- údaje jdou přímo srovnávat s **kótami na mapě** a s **výškovými hranicemi prostorů** vyjádřenými v nadmořské výšce (AMSL),
- QNH pro okolí zjistíš z meteorologických zpráv (METAR nejbližšího letiště) — mění se s počasím i během dne.

## QFE — výška nad místem

**QFE** je skutečný tlak v úrovni zvoleného místa (letiště, startoviště). Výškoměr nastavený na QFE ukazuje **výšku nad tímto místem** — na něm samotném ukazuje **nulu**. Je to intuitivní pro místní létání („mám 300 m nad startovačkou"), ale údaj nelze přímo srovnávat s mapou ani s hranicemi prostorů.

## QNE a letové hladiny — pro úplnost

Velká letadla ve výškách létají s výškoměrem nastaveným na standardní tlak **1013,25 hPa** (tzv. nastavení QNE); údaj se pak vyjadřuje jako **letová hladina (FL)**. Nad **převodní nadmořskou výškou** se přechází z QNH na standardní nastavení.

**⚠️ K verifikaci:** aktuální hodnotu převodní nadmořské výšky v ČR (uváděno 5 000 ft AMSL) a přesné definice Q-kódů ověř v AIP ČR / VFR příručce (aim.rlp.cz) a uveď zdroj.

## Postup na startovišti — prakticky

Pilot PK obvykle nemá radiové spojení s letištěm, QNH ale nastavíš i bez něj:

1. Zjisti **nadmořskou výšku startoviště** — z mapy (kóta), z databáze startovišť, z GPS.
2. **Otoč stavěcím prvkem výškoměru tak, aby ukazoval tuto nadmořskou výšku.** Tím máš nastaveno QNH, aniž bys znal číselnou hodnotu tlaku.
3. Chceš-li místo toho QFE, **vynuluj výškoměr na místě startu**.
4. Nastavení proveď **před každým letem** — tlak se během dne mění; ranní nastavení může odpoledne lhát o desítky metrů.

## Chyby a záludnosti

- **Změna tlaku za letu:** přiletíš-li na přeletu do oblasti s nižším tlakem, výškoměr **ukazuje víc, než skutečně máš** — letíš níž, než si myslíš. Pamatuj: „z vysokého do nízkého — pozor dolů".
- **Záměna QNH/QFE:** údaj „500 m" znamená při QNH nadmořskou výšku (nad mořem), při QFE výšku nad startovištěm. Záměna = chybný odhad výšky nad terénem i vůči prostorům. Vždy věz, s čím letíš.
- **Výška nad terénem se musí počítat:** výškoměr ti ji neukáže ani při jednom nastavení — spočítáš ji jako nadmořská výška (QNH) minus kóta terénu pod tebou z mapy.
- **Jednotky:** hranice prostorů na mapě ICAO jsou ve **ft**, tvůj výškoměr nejspíš v **m** — převod měj zažitý (1 000 ft ≈ 305 m).
- **GPS výška není náhrada:** liší se od barometrické o desítky metrů; vůči prostorům platí barometrická výška.

## Otázky k procvičení

<details>
<summary>Co ukazuje výškoměr nastavený na QNH a co na QFE?</summary>
<p>Při QNH ukazuje nadmořskou výšku (nad střední hladinou moře) — na startovišti tedy jeho kótu. Při QFE ukazuje výšku nad zvoleným místem — na něm samotném nulu.</p>
</details>

<details>
<summary>Jak nastavíš na startovišti QNH, když neznáš aktuální hodnotu tlaku?</summary>
<p>Zjistím nadmořskou výšku startoviště (kótu z mapy či databáze) a nastavím výškoměr tak, aby ji ukazoval — tím je nastaven na QNH bez znalosti číselné hodnoty tlaku.</p>
</details>

<details>
<summary>Proč je nutné výškoměr srovnat před každým letem?</summary>
<p>Protože atmosférický tlak se během dne mění — ranní nastavení může odpoledne ukazovat chybu i desítky metrů. Při přeletu do oblasti nižšího tlaku navíc výškoměr ukazuje víc, než skutečně letím.</p>
</details>

[← Zpět na Leteckou navigaci](../05-letecka-navigace.html#bod-7){: .btn-zpet}
